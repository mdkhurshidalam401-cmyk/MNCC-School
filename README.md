# HIKVENA PVT.LTD - School Management System 🎓

A comprehensive, role-based School Management System built to streamline administrative, academic, and financial operations. The system features strictly isolated portals for Admins, Teachers, Accountants, and Students with secure session management.

## 🚀 Features

*   **Secure Role-Based Access Control (RBAC):** Dedicated dashboards and isolated routing for Admin, Teacher, Accountant, and Student.
*   **Admin Workspace:** Manage overall school operations, staff, student admissions, fee structures, and approve/reject leave requests.
*   **Teacher Portal:** Manage assigned class rosters, mark daily student attendance, upload exam grades, and apply for leaves.
*   **Accounts/Finance Portal:** Process fee collections, track fee defaulters with direct WhatsApp reminders, manage operational expenses, and process staff payroll with monthly reports.
*   **Student Portal:** View personal daily attendance, check exam results, review fee payment history, and read live school notices.
*   **Live Notice Board:** Global and role-specific announcements pushed directly to respective dashboards.

## 🛠️ Tech Stack

*   **Frontend:** HTML5, Tailwind CSS (via CDN), FontAwesome Icons.
*   **Backend / Database:** Supabase (PostgreSQL) for real-time database management and querying.
*   **Authentication:** Custom JS logic with Supabase database matching and LocalStorage session guards.

## 📂 Key Modules

1.  **Authentication:** `login.html` (Verifies credentials directly from the Supabase `users` table).
2.  **Dashboards:** `index.html` (Admin), `teacher_dashboard.html`, `accountant_dashboard.html`, `student_dashboard.html`.
3.  **Academics:** Attendance, Exam Grading, Manage Subjects.
4.  **Finance:** Fee Collection, Defaulters List, Manage Expenses, Salary Payment, Salary Reports.
5.  **HR/Staff:** Staff Management, Leave Applications, Manage Leaves (Admin).

## ⚙️ Setup & Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/mdkhurshidalam401-cmyk/MNCC-School.git](https://github.com/mdkhurshidalam401-cmyk/MNCC-School.git)
    ```
2.  Open the project folder in your preferred code editor (e.g., VS Code).
3.  Configure your Supabase URL and Anon Key in the `script` tags across the HTML files.
4.  Ensure the following tables exist in your Supabase database:
    *   `users`
    *   `students`
    *   `staff`
    *   `attendance`
    *   `exam_marks`
    *   `fees_collection`
    *   `school_expenses`
    *   `salary_payments`
    *   `leave_requests`
    *   `notices`
5.  Run the project using a local server (like Live Server extension in VS Code) starting from `login.html`.