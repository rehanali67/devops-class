# 🎓 University Student Clubs Portal

A collaborative informational website for the fictional **UniConnect** Student Clubs Portal. Built as part of a DevOps team assignment demonstrating Git & GitHub collaborative workflows.

---

## 📁 Folder Structure

```
student-portfolio/
│
├── .gitignore
├── README.md
├── src/
│   ├── index.html        # Home / Landing page
│   ├── clubs.html        # Club categories
│   ├── events.html       # Upcoming events
│   ├── join.html         # Get involved / Join form
│   └── highlights.html   # Club highlights & spotlights
└── styles/
    └── style.css         # Shared stylesheet for all pages
```

---

## 🌐 Pages Overview

| Page | File | Description |
|------|------|-------------|
| Home | `src/index.html` | Welcome, hero section, quick navigation |
| Clubs | `src/clubs.html` | Club categories and descriptions |
| Events | `src/events.html` | Upcoming activities and schedules |
| Join | `src/join.html` | Application form and how to get involved |
| Highlights | `src/highlights.html` | Featured clubs and student testimonials |

---

## 🌿 Git Branching Strategy

```
main (production)
└── release (QA / staging)
    └── develop (active development)
        ├── feature/home-page
        ├── feature/clubs-page
        ├── feature/events-page
        ├── feature/join-page
        └── feature/highlights-page
```

### Branch Rules
- **`main`** — Production-ready code only. Merged from `release` after QA sign-off.
- **`release`** — QA/staging branch. Merged from `develop` before production.
- **`develop`** — Active development branch. All feature branches merge here first.
- **`feature/*`** — Individual feature branches created by each team member.

---

## 🔄 Workflow for Team Members

1. **Clone** the repository:
   ```bash
   git clone <repo-url>
   cd student-portfolio
   ```

2. **Checkout `develop`** and pull the latest:
   ```bash
   git checkout develop
   git pull origin develop
   ```

3. **Create your feature branch** from `develop`:
   ```bash
   git checkout -b feature/your-page-name
   ```

4. **Make changes**, then stage and commit:
   ```bash
   git add .
   git commit -m "feat: add [page-name] page content"
   ```

5. **Rebase onto `develop`** before pushing (to keep history clean):
   ```bash
   git fetch origin
   git rebase origin/develop
   ```

6. **Push** your branch and open a **Pull Request** to `develop`:
   ```bash
   git push origin feature/your-page-name
   ```

7. **Request a review** from the Team Lead before merging.

---

## 🧰 Technologies Used

- **HTML5** — Semantic markup
- **CSS3** — Shared stylesheet with responsive design via media queries
- **Git & GitHub** — Version control and collaborative workflow

---

## 👥 Team Responsibilities

| Role | Responsibility |
|------|----------------|
| Team Lead | Repo init, folder structure, `main` / `release` / `develop` branches, CSS base |
| Member 1 | `index.html` — Home page |
| Member 2 | `clubs.html` — Club categories |
| Member 3 | `events.html` — Upcoming events |
| Member 4 | `join.html` — Join / contact form |
| Member 5 | `highlights.html` — Club highlights |

---

## 📝 Commit Message Convention

```
feat:     New feature or page
fix:      Bug fix
style:    CSS / UI changes
docs:     README or documentation
chore:    Repo maintenance (gitignore, folder setup)
```

---

*Made with ❤️ for DevOps Collaborative Git Assignment*
