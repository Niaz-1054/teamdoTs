# 🎓 UGV Result Analysis & GPA Dashboard

A data‑driven academic platform for **University of Global Village (UGV)** that enables students, teachers, and administrators to **analyze results, track GPA/CGPA trends, and manage academic records** through a clean UI.

---

## 🚀 Project Overview

**UGV Result Analysis & GPA Dashboard** is a full‑stack academic analytics system designed to:

- Analyze **semester‑wise GPA trends**
- Calculate **CGPA accurately (max 4.0)**
- Provide **personalized academic insights**
- Manage **student enrollments, subjects, and grades**
- Support **Admin, Teacher, and Student roles**

The system uses **realistic academic data** to simulate a real university environment suitable for evaluations, and future expansion.

---

## ✨ Key Features

### 👩‍🎓 Student
- View **CGPA & GPA trend**
- Semester‑wise result breakdown
- **Top 3 strong subjects**
- Personalized improvement recommendations
- GPA simulation 

### 👨‍🏫 Teacher
- View enrolled students per subject & semester
- Enter and update grades securely
- Subject‑wise performance overview

### 🧑‍💼 Admin
- Student enrollment management (scroll‑based, compact UI)
- Assign teachers to subjects & semesters
- Manage semesters, sessions, and subjects
- Full academic data visibility

---

## 🧠 Academic Logic (UGV‑Specific)

- **Sessions used:** `Summer <Year>` and `Winter <Year>`
- Supports **multi‑semester students** (1st → 8th semester)
- CGPA is always **≤ 4.0**
- GPA trends are **chronologically ordered**
- All enrollments, transcripts, and analytics are **fully connected**

---

## 🛠️ Tech Stack

**Frontend**
- React + TypeScript (`.tsx`)
- Vite
- Modern component‑based architecture
- Apple‑style minimal UI

**Backend**
- Supabase (PostgreSQL)
- Row Level Security (RLS)
- Foreign key–safe relational schema

---

## 🧩 Database Highlights

- `profiles` — students, teachers, admins  
- `enrollments` — student ↔ subject ↔ semester  
- `teacher_assignments` — teacher ↔ subject ↔ semester  
- `transcripts` — grades & GPA data  
- `semesters` & `sessions` — academic timeline  

✔ No orphan records  
✔ Left‑join safe queries  
✔ Demo‑friendly RLS policies  

---

## 🖥️ UI & Branding

- Official **University of Global Village (UGV)** branding
- Clean typography and spacing
- Non‑intrusive, professional layout

---

## 📦 Project Setup (Local)

```sh
# Clone the repository
git clone (https://github.com/Niaz-1054/teamdoTs]
# Navigate to the project directory
cd <teamdoTs>

# Install dependencies
npm install
# Start the development server
npm run dev
``

The application will be available at `http://localhost:8080`

## Project Structure

```
src/
├── components/     # Reusable UI components
│   ├── admin/      # Admin-specific components
│   ├── auth/       # Authentication components
│   ├── layout/     # Layout components
│   ├── student/    # Student dashboard components
│   ├── teacher/    # Teacher dashboard components
│   └── ui/         # shadcn/ui components
├── contexts/       # React contexts
├── hooks/          # Custom hooks
├── integrations/   # External service integrations
├── lib/            # Utility functions
└── pages/          # Page components
```

## License

This project was developed by TEAMdoTs as part of UNIBUILD-36 hackathon submission.
