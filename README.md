# 🗳️ Automated Voting System

A secure and user-friendly web application that digitizes small-scale elections such as college elections, organizational voting, and internal decision polls. The system provides role-based access, real-time result counting, and ensures one-vote-per-user authentication.

---

## 🧑‍💻 Tech Stack (Languages Used)

This project is primarily based on web technologies with a strong focus on interactive UI, secure backend, and responsive styling.

| Language / Tech | Usage | Percentage |
|----------------|------|-----------|
| **JavaScript** | Frontend interactivity, form validation, AJAX requests | **53.2%** |
| **PHP** | Server-side logic, authentication, vote processing, DB operations | **21.9%** |
| **SCSS** | Component-based styling, UI consistency | **10.5%** |
| **LESS** | Theming and structured CSS management | **10.4%** |
| **CSS** | Global styling and layout | **3.3%** |
| **Hack** | Minor backend/legacy modules | **0.7%** |

> ✔️ Frontend heavy  
> ✔️ PHP backend  
> ✔️ Modern styling using SCSS & LESS  

---

## 🚀 Key Features

- **User Registration & Login**
- **Admin & Voter Roles**
- **Create and Manage Elections**
- **Candidate & Party Management**
- **Secure Vote Casting (One user = One vote)**
- **Real-time Vote Counting**
- **Dashboard for Admin**
- **Result Visualization (tables/charts)**

---

## 📂 Modules

### 👤 Admin
- Create elections
- Add candidates
- Approve voter accounts
- Monitor live results

### 🧑‍💼 Voter
- Login
- View active elections
- Cast vote once per election
- Vote confirmation screen

---

## 🗄️ Database Overview

**Tables**

- `users`
- `elections`
- `candidates`
- `votes`

**Important Constraints**
- Unique `(voter_id, election_id)` pair → prevents duplicate voting

---

## 🔐 Security

- Password hashing (PHP `password_hash()`)
- Session-based authentication
- CSRF protection for forms
- Vote time validation (only active elections allowed)

---

## 🧰 Installation & Setup

### Requirements
- PHP 7+
- MySQL / MariaDB
- Apache / Nginx
- Node.js (optional for SCSS/LESS build)

### Steps

```bash
# Clone
git clone https://github.com/<your-username>/Automated-Voting-System.git

# Move to project folder
cd Automated-Voting-System
