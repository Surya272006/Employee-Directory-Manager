# 👨‍💼 Employee Directory Manager

A simple **CRUD-based employee record management system** written in Python. It lets you **Create, Read, Update and Delete** employee records through a menu-driven console program, and also includes a **Streamlit web interface** with the same functionality.

> Academic project – B.Tech CSE (AIML), Semester III, Year 2nd – **Group C**

---

## 📌 Table of Contents

- [Features](#-features)
- [Data Structure](#-data-structure)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Menu Options](#-menu-options)
- [Sample Data](#-sample-data)
- [Limitations](#-limitations)
- [Future Scope](#-future-scope)


---

## ✨ Features

- ➕ **Add** a new employee with a unique Employee ID
- 📋 **View** all employees in a neat table
- 🔍 **Search** an employee by ID
- ✏️ **Update** an existing record (console version: press Enter to keep the old value)
- 🗑️ **Delete** an employee record
- ✅ Input checks for empty ID/name and duplicate IDs
- 💬 Clear success and error messages for every action
- 🌐 Two interfaces: **Console** and **Streamlit web app**

## 🛠 Tech Stack

| Component | Details |
|---|---|
| Language | Python 3.x |
| Web Framework | Streamlit (for the web version) |
| Editor | Visual Studio Code |
| Version Control | Git & GitHub |

## 🧱 Data Structure

Employees are stored in a Python **dictionary**. The key is the Employee ID and the value is a **tuple** of the remaining details:

```python
directory[emp_id] = (name, role, birthdate, joining_date, salary)
```

A dictionary gives fast lookup by ID and prevents duplicate IDs, while tuples keep each record compact.

## 📂 Project Structure

```
Employee-Directory-Manager/
├── emp_director.py     # Console (menu-driven) version
├── app.py              # Streamlit web version (rename to match your file)
├── screenshots/        # Output screenshots used in this README
└── README.md
```

> **Note:** Change `app.py` above to the actual file name of your Streamlit program.

## ⚙️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Surya272006/Employee-Directory-Manager.git
   cd Employee-Directory-Manager
   ```

2. **Make sure Python 3 is installed**

   ```bash
   python --version
   ```

3. **Install Streamlit** (only needed for the web version)

   ```bash
   pip install streamlit
   ```

## ▶️ How to Run

**Console version**

```bash
python emp_director.py
```

**Streamlit web version**

```bash
streamlit run app.py
```

The app opens in your browser at `http://localhost:8501`.

## 📖 Menu Options

**Console version**

```
--- Employee Directory Manager ---
Enter 1 Add Employee (Create)
Enter 2 View All Employees (Read)
Enter 3 Search Employee by ID (Read)
Enter 4 Update Employee (Update)
Enter 5 Delete Employee (Delete)
Enter 6 Exit
```

**Streamlit version** – choose an action from the sidebar: *View All Employees, Add Employee, Search Employee, Update Employee, Delete Employee*.

## 🖼 Screenshots

| Operation | Screenshot |
|---|---|
| Add Employee | ![Add](screenshots/01-add-employee.png) |
| View All Employees | ![View](screenshots/02-view-all.png) |
| Search Employee | ![Search](screenshots/03-search.png) |
| Update Employee | ![Update](screenshots/04-update.png) |
| Delete Employee | ![Delete](screenshots/05-delete.png) |
| Exit | ![Exit](screenshots/06-exit.png) |

## 🔄 Flow Chart

![Flow Chart](screenshots/flowchart.png)

## 🗂 Sample Data

The program starts with four sample records:

| ID | Name | Role | Birthdate | Joining Date | Salary |
|---|---|---|---|---|---|
| E101 | Subhadip Koley | Software Engineer | 06/06/2006 | 27/08/2020 | 50k |
| E102 | Rahul Podder | Machine Learning Engineer | 17/11/2005 | 06/05/2017 | 90k |
| E103 | Surya Samanta | Information Technology | 27/12/2006 | 12/11/2023 | 30k |
| E104 | Sudipta Das | AI Engineer | 22/12/2005 | 30/06/2022 | 40k |

## ⚠️ Limitations

- Data is stored **in memory only** and is lost when the program or session ends.
- Date and salary fields are plain text with no format validation.
- No login system or role-based access control.

## 🚀 Future Scope

- Store data permanently using SQLite / MySQL
- Add date and salary validation
- Add authentication and search by name or role
- Export records to CSV / PDF
- Deploy the Streamlit app online

## 👥 Team Members

**Group C – B.Tech CSE (AIML), Semester III**

| Name | Student Code |
|---|---|
| Subhadip Koley | BWU/BTA/25/648 |
| Surya Samanta | BWU/BTA/25/646 |
| Sudipta Das | BWU/BTA/25/654 |
| Rahul Poddar | BWU/BTA/25/643 |

---

⭐ If you found this project useful, consider giving the repository a star!
