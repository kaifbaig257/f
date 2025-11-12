🎓 Campus Events Website – DevOps Assignment 02 (Fall 2025)Welcome to the Campus Events repository. This project was developed as part of DevOps Fundamentals (Fall 2025) to demonstrate a comprehensive understanding of Git workflow, branching strategy, pull requests, rebasing, Docker image creation, and release management using GitHub.🚀 Project OverviewThe Campus Events Website is a responsive, multi-page static platform designed to highlight and manage upcoming university events, seminars, and workshops.The website provides an engaging interface where students can:Explore academic and extracurricular eventsStay informed about new opportunitiesConnect with departments and organizers💻 Technologies UsedThis project is built with:Frontend: HTML5, CSS3Build Tool: Parcel (for bundling static assets)Containerization: DockerDevOps Workflow: Git, GitHub (Branches, PRs, Actions)🛠️ Getting StartedFollow these instructions to get a copy of the project up and running on your local machine for development and testing.PrerequisitesYou will need the following tools installed on your system:GitNode.js (which includes npm)Docker (optional, for container-based setup)Installation & Local DevelopmentClone the repository:Bashgit clone https://github.com/DevOps-Fundamentals/campus-events.git
cd campus-events
Install dependencies:This project uses package.json to manage development dependencies like Parcel.Bashnpm install
Run the development server:This command will start a local server with hot-reloading.Bashnpm run dev
You can now view the website at http://localhost:1234.Build for production:This command will bundle the site into the dist/ directory.Bashnpm run build
🐳 Running with DockerYou can also build and run this project as a Docker container.Build the Docker image:From the root of the project, run:Bashdocker build -t campus-events .
Run the Docker container:This command runs the built image, mapping port 8080 on your local machine to port 80 in the container.Bashdocker run -d -p 8080:80 campus-events
You can now view the website at http://localhost:8080.📁 Folder Structurecampus-events/
|
├── .dockerignore       # Files to ignore for Docker build
├── .gitignore          # Files to ignore for Git
├── Dockerfile          # Instructions to build the Docker image
├── README.md           # This file
├── package.json        # Project metadata and dependencies
|
├── src/                # Main source code
│   ├── index.html
│   ├── about.html
│   ├── events.html
│   ├── gallery.html
│   ├── contact.html
│   └── faq.html
│
│── assets/
│   └── images/
│       └── hero-campus.jpg
│
├── styles/
│   └── style.css
│
└── dist/               # Auto-generated build output
Each page (.html) was developed on a separate feature branch and merged into the develop branch via protected pull requests.👥 Team Roles & ResponsibilitiesRoleNameResponsibilitiesTeam LeadAbdul Wahab SubhaniDevelops index.html, repo setup, branch protection, issue creation, release managementMember 1Muhammad AhmadDevelops about.html pageMember 2Yasir IftikharDevelops events.html pageMember 3Abdul Wahab SubhaniDevelops gallery.html pageMember 4Kaif BaigDevelops contact.html pageMember 5Umar DrazDevelops faq.html page🧩 Git & GitHub WorkflowMain Branchesmain → Production-ready branch.develop → Integration branch for testing and staging.Feature Branch Naming ConventionEach feature or page is developed under its own branch:feature/indexfeature/aboutfeature/eventsfeature/galleryfeature/contactfeature/faqBranch Protection Rules❌ No direct pushes allowed to develop or main.✅ Pull Requests (PRs) are required for every merge.🔒 develop → requires 2 approvals.🔒 main → requires 3 approvals.🧹 All PRs must be rebased before merging to maintain a clean Git history.
