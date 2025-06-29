## 🎓 Student Management System – Bash Script

A command-line based **Student Management System** written in pure `bash` that allows teachers to manage student data and students to view their academic details. Features include CGPA calculation, sorting, grade evaluation, secure login, and more.

---

## 📂 Features

### 👨‍🏫 Teacher Panel

* Add up to 20 students with names and roll numbers
* Remove students
* Update student information (name, class, marks)
* Automatically calculates GPA and CGPA from marks
* View student details
* Sort students by GPA (ascending/descending)
* View passed or failed students (based on GPA threshold)

### 👨‍🎓 Student Panel

* Secure login via roll number and password
* First-time login forces password update
* View detailed marks and grades

---

## 🗂️ File Structure

* `new_final.sh` – Main script (run this file)
* `studentfile.txt` – Stores student records (CSV format)
* `credentials.txt` – Stores student login credentials (`roll,password`)

---

## 🛠️ Requirements

* Unix/Linux environment
* `bash` shell
* `awk`, `bc`, `sed`, and `sort` utilities installed

---

## ▶️ How to Run

1. Make the script executable:

   ```bash
   chmod +x new_final.sh
   ```

2. Run the script:

   ```bash
   ./new_final.sh
   ```

---

## 📝 Data Format

Each student is stored in `studentfile.txt` as:

```text
Name,RollNumber,Class,MathMarks,OSMarks,DBMarks,GPA
```

Example:

```
Ali Raza,101,BSCS,85,90,88,3.63
```

---

## 🔐 Login Info

### Default Teacher Login

* **Username:** `admin`
* **Password:** `123`

### Student Login

* Students are added by the teacher
* Default password: `123` (must be changed on first login)

---

## ⚙️ Functional Overview

* **Grades** are calculated as per the numerical score using a predefined grading scale (A+, A, B, ..., F)
* **GPA** is derived from marks using a linear conversion
* **CGPA** is computed as the average of three subject GPAs

---

## 💡 Future Improvements (Suggestions)

* Add file backup and restore
* Encrypt passwords
* Add subject-wise analytics or class averages
* GUI interface via `dialog` or Zenity

---

## 📄 License

This project is open source and free to use for educational purposes.


