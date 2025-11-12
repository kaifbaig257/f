🎓 Campus Events Website – DevOps Assignment 02 (Fall 2025)

Welcome to the Campus Events repository. This project was developed as part of DevOps Fundamentals (Fall 2025) to demonstrate a comprehensive understanding of Git workflow, branching strategy, pull requests, rebasing, Docker image creation, and release management using GitHub.
🚀 Project Overview

The Campus Events Website is a responsive, multi-page static platform designed to highlight and manage upcoming university events, seminars, and workshops.

The website allows students to:

Explore academic and extracurricular events

Stay informed about new opportunities

Connect with departments and organizers

💻 Technologies Used

Frontend: HTML5, CSS3

Build Tool: Parcel (for bundling static assets)

Containerization: Docker

DevOps Workflow: Git, GitHub (Branches, PRs, Actions)

🛠️ Getting Started

Follow these instructions to get a copy of the project running locally for development and testing.

Prerequisites

Ensure the following tools are installed:

Git

Node.js (includes npm)

Docker (optional, for container setup)

Installation & Local Development

Clone the repository

git clone https://github.com/DevOps-Fundamentals/campus-events.git
cd campus-events


Install dependencies

npm install


Run the development server

npm run dev


Access the website at: http://localhost:1234

Build for production

npm run build


Bundled files will be generated in the dist/ directory.

🐳 Running with Docker
Build the Docker image
docker build -t campus-events .

Run the Docker container
docker run -d -p 8080:80 campus-events


Access the website at: http://localhost:8080

📁 Folder Structure
campus-events/
│
├── .dockerignore       # Files to ignore for Docker build
├── .gitignore          # Files to ignore for Git
├── Dockerfile          # Instructions to build the Docker image
├── README.md           # Project documentation
├── package.json        # Project metadata and dependencies
│
├── src/                # Main source code
│   ├── index.html
│   ├── about.html
│   ├── events.html
│   ├── gallery.html
│   ├── contact.html
│   └── faq.html
│
├── assets/
│   └── images/
│       └── hero-campus.jpg
│
├── styles/
│   └── style.css
│
└── dist/               # Auto-generated build output


Each page was developed on a separate feature branch and merged into the develop branch via protected pull requests.

👥 Team Roles & Responsibilities
Role	Name	Responsibilities
Team Lead	Abdul Wahab Subhani	Develops index.html, repo setup, branch protection, issue creation, release management
Member 1	Muhammad Ahmad	Develops about.html
Member 2	Yasir Iftikhar	Develops events.html
Member 3	Abdul Wahab Subhani	Develops gallery.html
Member 4	Kaif Baig	Develops contact.html
Member 5	Umar Draz	Develops faq.html
🧩 Git & GitHub Workflow
Main Branches

main → Production-ready branch

develop → Integration branch for testing and staging

Feature Branch Naming Convention

Each feature or page is developed under its own branch:

feature/index
feature/about
feature/events
feature/gallery
feature/contact
feature/faq

Branch Protection Rules

❌ No direct pushes allowed to develop or main.

✅ Pull Requests (PRs) required for every merge.

🔒 develop → Requires 2 approvals

🔒 main → Requires 3 approvals

🧹 All PRs must be rebased before merging to maintain a clean Git history.
