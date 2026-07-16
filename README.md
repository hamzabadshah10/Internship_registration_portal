<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=Internship%20Portal&fontSize=60&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=PHP%20%7C%20MySQL%20%7C%20Web%20Security&descAlignY=60&descAlign=50" width="100%"/>

<br/>

# 🔒 PAF-IAST Secure Internship Registration Portal - University Project

### *A robust, secure, and visually modern web portal for student industry placements.*

<br/>

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=for-the-badge)](https://github.com/hamzabadshah10/Internship_registration_portal)
[![PHP](https://img.shields.io/badge/PHP-8.0+-777BB4.svg?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Security](https://img.shields.io/badge/Security-Multi--Layered-success.svg?style=for-the-badge)](https://github.com/hamzabadshah10/Internship_registration_portal)

<br/>

[![GitHub Stars](https://img.shields.io/github/stars/hamzabadshah10/Internship_registration_portal?style=for-the-badge&logo=github&color=ffd700)](https://github.com/hamzabadshah10/Internship_registration_portal/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/hamzabadshah10/Internship_registration_portal?style=for-the-badge&logo=github&color=4fc3f7)](https://github.com/hamzabadshah10/Internship_registration_portal/network)
[![GitHub Issues](https://img.shields.io/github/issues/hamzabadshah10/Internship_registration_portal?style=for-the-badge&logo=github&color=ff7043)](https://github.com/hamzabadshah10/Internship_registration_portal/issues)
[![License](https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge)](LICENSE)

</div>

---

## 👩‍💻 About This Repository

This project provides a robust, highly secure, and visually modern web portal designed for software engineering students at **Pak-Austria Fachhochschule (PAF-IAST)** to register for industry internship placements. It emphasizes strict data integrity, multi-level form validation, and defense against common web vulnerabilities, all wrapped in a premium "Glassmorphism" user interface.

<div align="center">
  <img width="80%" alt="Form Preview" src="https://github.com/user-attachments/assets/40fa497e-e147-4b5f-a746-0523a106deda" />
</div>

---

## 🚀 Key Features

* **Real-Time AJAX Validation:** Live checking of university email availability before form submission to prevent duplicate entries.
* **Multi-Level Security:** 
  * Client-side Regex validation for immediate user feedback.
  * Server-side PHP re-validation to ensure data integrity even if JavaScript is bypassed.
* **Secure File Handling:** Resume uploads are strictly restricted to `.pdf` formats using true MIME-type validation via `finfo_file` (preventing `.php` files renamed to `.pdf`), with a 2MB size limit and `.htaccess` execution prevention.
* **Threat Prevention:** 
  * **SQL Injection (SQLi):** Mitigated using PDO Prepared Statements.
  * **Cross-Site Scripting (XSS):** Mitigated using strict input sanitization (`htmlspecialchars`).
* **Modern UI/UX:** Responsive, fully custom Midnight Slate & Ocean Blue CSS theme featuring glassmorphism cards, dynamic focus states, and intuitive placeholder hints.

---

## 🧠 Skills & Technologies

<div align="center">

### Core Stack
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

### Concepts Covered
![Web Security](https://img.shields.io/badge/Web%20Security-6f42c1?style=flat-square)
![Form Validation](https://img.shields.io/badge/Form%20Validation-6f42c1?style=flat-square)
![Glassmorphism](https://img.shields.io/badge/UI/UX-6f42c1?style=flat-square)

</div>

---

## 🚀 Quick Start

1. **Clone the Repository:**
   Place the project folder into your local server's web directory (`C:\xampp\htdocs\` or `C:\wamp64\www\`).
   ```bash
   git clone https://github.com/hamzabadshah10/Internship_registration_portal.git
   ```

2. **Database Configuration:**
   * Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
   * Create a new database named `university_portal`.
   * Run the provided SQL to generate the schema with proper integrity constraints.

3. **Launch the Portal:**
   * Start your Apache and MySQL servers.
   * Access the portal at `http://localhost/Internship_registration_portal`.

---

## 🤝 Connect & Contribute

<div align="center">

[![GitHub Follow](https://img.shields.io/github/followers/hamzabadshah10?label=Follow%20on%20GitHub&style=for-the-badge&logo=github&color=181717)](https://github.com/hamzabadshah10)
[![Star Repo](https://img.shields.io/badge/⭐%20Star%20This%20Repo-ffd700?style=for-the-badge)](https://github.com/hamzabadshah10/Internship_registration_portal/stargazers)
[![Fork Repo](https://img.shields.io/badge/🍴%20Fork%20This%20Repo-4fc3f7?style=for-the-badge)](https://github.com/hamzabadshah10/Internship_registration_portal/fork)

</div>

Feel free to explore, fork, or reach out with any questions! If you found this repo helpful, please **⭐ star it** — it means a lot! 🙏

---

## 📄 License

Distributed under the **MIT License** — free to use, share, and adapt with attribution.

---

<div align="center">

### 👩‍💻 Author

**Hamza Badshah**
*Software Engineering Department, PAF-IAST*

[![GitHub](https://img.shields.io/badge/GitHub-hamzabadshah10-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/hamzabadshah10)

<br/>

*Securing digital portals for the modern web.*

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

</div>
