# Online Course Application - Exam & Assessment Feature

This repository contains the Django full-stack implementation for adding an **Assessment/Exam Feature** to an existing Online Course Application. This project is part of the IBM Full Stack Developer / Django Application Development curriculum on Cognitive Class and Coursera.

---

## 📌 Project Overview

The goal of this project is to extend an existing online learning management system (LMS) by designing and integrating an automated assessment tool. Key implementations include:

- **Data Models:** Created `Question`, `Choice`, and `Submission` models linked to courses and user enrollments.
- **Admin Panel:** Integrated inline forms (`QuestionInline`, `ChoiceInline`) and custom admin classes (`QuestionAdmin`, `LessonAdmin`) for course creators.
- **Exam Interface:** Added dynamic exam forms to course detail templates using Bootstrap styling and Django template tags.
- **Evaluation & Views:** Developed view handlers (`submit` and `show_exam_result`) to calculate grades dynamically based on user selections.

---

## 🛠️ Project Structure

```text
onlinecourse/
├── admin.py                    # Admin site registrations and inline models
├── models.py                   # Data models (Course, Question, Choice, Submission, etc.)
├── urls.py                     # URL routing for exam submission and results
├── views.py                    # Logic for handling exam submissions and scoring
└── templates/
    └── onlinecourse/
        ├── course_details_bootstrap.html  # Course detail & exam form view
        └── exam_result_bootstrap.html     # Exam results view
