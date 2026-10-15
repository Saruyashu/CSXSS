<div align="center">

# 🎓 CSXSS — Unified Campus Platform

**CampuShare × SkillSwap: one place for students to share, learn and connect.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![JSP](https://img.shields.io/badge/JSP-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Status](https://img.shields.io/badge/status-in_development-yellow?style=for-the-badge)

</div>

---

## 📖 About

CSXSS is a campus web platform that combines two ideas under one login:

- **CampuShare** is a campus marketplace where students list and find academic items, so they *share more, spend less and waste less*.
- **SkillSwap** is a peer-to-peer learning space with courses, mentorship and communities.

## ✨ Features

| Module | What it does |
|---|---|
| 🛒 **CampuShare** | Browse the campus marketplace and list an academic item (`CampuShare.html`, `listing.html`) |
| 📚 **E-Library** | Study resources in one place (`E-Library.html`) |
| 🧑‍🏫 **Mentorship** | Peer-to-peer mentor directory and mentor registration (`mentorship_directory.html`, `mentor_registration_form.html`) |
| 🎯 **Courses** | "Upskill with Campus Experts" course listings (`courses.html`) |
| 👥 **Communities** | Campus community pages (`community_page.html`) |
| 🔐 **Accounts** | Registration and login backed by a MySQL table (`Registrationpg.html`, `Login.html`, `validate.jsp`) |

## 🧱 Tech Stack

- **Frontend:** HTML5 and [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- **Backend:** Java Server Pages (JSP) with JDBC
- **Database:** MySQL
- **Server:** Apache Tomcat (or any servlet container)

## 🗂️ Project Structure

```
csxss/
├── HomePg.html                  # Landing page
├── AbtUs.html · Service.html    # About and services
├── Login.html · Registrationpg.html
├── CampuShare.html · listing.html
├── E-Library.html
├── courses.html
├── community_page.html
├── mentorship_directory.html · mentor_registration_form.html
├── validate.jsp                 # Login check against the database
├── mentor-validation.jsp        # Mentor form handling
└── logo.svg · clogo.svg · slogo.svg
```

## 🚀 Getting Started

1. **Clone the repo**
   ```bash
   git clone https://github.com/Saruyashu/CSXSS.git
   ```
2. **Static pages only:** open `HomePg.html` in your browser. No build step is needed.
3. **With login and mentor features (JSP):**
   - Install JDK 17+, Apache Tomcat 9+ and MySQL 8+.
   - Create the database and tables used by `validate.jsp` and `mentor-validation.jsp`.
   - Add a `csxss.DatabaseConnection` class with your own database credentials. Keep credentials out of version control.
   - Deploy the folder as a web app on Tomcat and open `http://localhost:8080/<app-name>/HomePg.html`.

## 🛣️ Roadmap

- [ ] Hash passwords before storing them
- [ ] Add the database schema and a setup script to the repo
- [ ] Connect the marketplace listing form to the database
- [ ] Add a student dashboard

## 🤝 Contributing

Ideas and pull requests are welcome. Open an issue first to discuss any larger change.

## 👤 Author

Built by [@Saruyashu](https://github.com/Saruyashu).
