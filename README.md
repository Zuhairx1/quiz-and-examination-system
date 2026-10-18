# Quiz and Examination System

A Q & A system which features an examination and a quiz.
An online quiz/exam creation, management and attempt system. It does away with manual paper based testing and evaluates them automatically.

Course project of Software Construction and Development.

## Group Members

| Name | GitHub Username | Initial Responsibility |
|------|-----------------|------------------------|
| Abdur Rahim Ajmal | [@abdurrahim-07](https://github.com/abdurrahim-07) | Backend core, authentication, Admin module |
| Zuhair Nasir | [@Zuhairx1](https://github.com/Zuhairx1) | Question banks, quiz engine, randomization, grading and unit tests |
| Somna Imran | [@somnaimran](https://github.com/somnaimran) | MySQL schema, HTML/CSS interface, attempt page, proctoring UI |

## Overview
User roles

Admin - User and System Management.
Teacher - Creates quizzes, manages the questions, sees the results.
Student - takes quizzes and checks their scores and history.

**Core features**

MCQ and True/False questions
Timed exams with auto-submit
Instant automatic grading
Alternative question banks (where each student is provided with a different set but they are all random)
The basic online exam monitoring features include tab-switch, full-screen and copy/paste detection.

## Technology
Python Flask, MySQL, HTML, CSS (and some basic JavaScript for the timer and monitoring).

## Project Structure

## Project Structure

```
quiz-exam-system/
├── README.md
├── requirements.txt
├── config.py
├── run.py
├── docs/            requirements document and design notes
├── database/        schema.sql, seed.sql
├── app/
│   ├── routes/      auth, admin, teacher, student
│   ├── services/    grading, randomizer, proctoring
│   ├── models/      database access
│   ├── templates/   HTML pages
│   └── static/      css, js
└── tests/           unit tests (pytest)
```

## Conventions

Files, folders and database tables: lowercase snake_case.
Pull requests to merge changes.Feature/name or fix/name.
Commits: feat:, fix:, docs:, test:, refactor: and then followed by a short description.
Versions: Git tags v0.1.0, v0.2.0 ... v1.0.0 (first complete release).

## Documentation

[Requirements document](docs/Requirements_Document_Quiz_Exam_System.docx)

## Current Status

**v0.1.0 - project initiation.** Created repository, identified requirements and added to product backlog. Next: Database schema, login and role based access (see backlog in requirements document).