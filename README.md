🎓 PAF-IAST Secure Internship Registration Portal

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![PHP](https://img.shields.io/badge/PHP-8.0+-777BB4.svg?logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1.svg?logo=mysql&logoColor=white)
![Security](https://img.shields.io/badge/Security-Multi--Layered-success.svg)


<img width="959" height="512" alt="FORM" src="https://github.com/user-attachments/assets/40fa497e-e147-4b5f-a746-0523a106deda" />


<img width="959" height="510" alt="SUBMITTED" src="https://github.com/user-attachments/assets/bdef52c8-1f19-4616-8f72-04d0d9aeb258" />



A robust, highly secure, and visually modern web portal designed for software engineering students at Pak-Austria Fachhochschule (IAST) to register for industry internship placements. 

This project emphasizes strict data integrity, multi-level form validation, and defense against common web vulnerabilities, all wrapped in a premium "Glassmorphism" user interface.

## ✨ Key Features

* **Real-Time AJAX Validation:** Live checking of university email availability before form submission to prevent duplicate entries.
* **Multi-Level Security:**  Client-side Regex validation for immediate user feedback.
    * Server-side PHP re-validation to ensure data integrity even if JavaScript is bypassed.
* **Secure File Handling:** Resume uploads are strictly restricted to `.pdf` formats using true MIME-type validation via `finfo_file` (preventing `.php` files renamed to `.pdf`), with a 2MB size limit and `.htaccess` execution prevention.
* **Threat Prevention:**  **SQL Injection (SQLi):** Mitigated using PDO Prepared Statements.
    * **Cross-Site Scripting (XSS):** Mitigated using strict input sanitization (`htmlspecialchars`).
* **Modern UI/UX:** Responsive, fully custom Midnight Slate & Ocean Blue CSS theme featuring glassmorphism cards, dynamic focus states, and intuitive placeholder hints.

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3 (Custom Grid/Flexbox UI), Vanilla JavaScript (AJAX, DOM Manipulation)
* **Backend:** PHP (PDO)
* **Database:** MySQL
* **Testing/Environment:** XAMPP / WAMP Server

## 🚀 Installation & Setup

1. **Clone or Download the Repository:**
   Place the `Secure_Internship_Portal` folder into your local server's web directory (e.g., `C:\xampp\htdocs\` for XAMPP or `C:\wamp64\www\` for WAMP).

2. **Database Configuration:**
   * Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
   * Create a new database named `university_portal`.
   * Run the following SQL to generate the schema with proper integrity constraints:
     ```sql
     CREATE TABLE students (
         id INT AUTO_INCREMENT PRIMARY KEY,
         student_id VARCHAR(20) NOT NULL UNIQUE,
         full_name VARCHAR(100) NOT NULL,
         email VARCHAR(100) NOT NULL UNIQUE,
         password VARCHAR(255) NOT NULL,
         cnic VARCHAR(15) NOT NULL UNIQUE,
         phone VARCHAR(11) NOT NULL,
         cgpa DECIMAL(3,2) NOT NULL CHECK (cgpa BETWEEN 0.00 AND 4.00),
         department VARCHAR(50) NOT NULL,
         resume_path VARCHAR(255) NOT NULL,
         registration_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
     ) ENGINE=InnoDB;
     ```

3. **Directory Permissions:**
   Ensure the `uploads/` directory exists in the root folder and is writable. A `.htaccess` file is automatically generated inside it upon the first upload to prevent script execution.

4. **Launch the Application:**
   Open your web browser and navigate to: `http://localhost/Secure_Internship_Portal/index.html`

## 🛡️ Security Architecture 
This system was built with a "Zero Trust" architecture regarding user input:
* **What happens if JavaScript is disabled?** The system remains secure. Client-side JS is purely for UX. The `register.php` file independently re-validates all regex patterns, file sizes, and data types before interacting with the database.
* **Password Storage:** Plain-text passwords are never stored. They are hashed using the strong `BCRYPT` algorithm via PHP's `password_hash()`.

## 👨‍💻 Author

**Hamza Badshah**

**Software Engineer | Pak-Austria Fachhochschule Institute of Applied Sciences and Technology**

---

*Developed for Web Engineering coursework. Built for security, designed for usability.*
