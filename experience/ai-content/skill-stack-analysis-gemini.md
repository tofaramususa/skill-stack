Backend Development & Programming:

Python: Implied by the context of API development, backend logic, and scripting for tasks like interacting with workflows and data manipulation. Specific mentions include "python packages."
API Development (General): Significant experience in designing, developing, and iterating on APIs (e.g., "Snapshots API service," "deepResearcher API endpoint"). This includes:
API Specification: Creating initial specs and iterating based on feedback.
Endpoint Design: Designing various GET/POST endpoints for different functionalities (products, folders, prompts, reports, tasks, user auth, etc.).
CRUD Operations: Implementing Create, Read, Update, Delete functionalities for various data models.
Error Handling: Implementing error handling for backend endpoints.
API Documentation: Creating API docs (e.g., using tools integrated with the production environment).
Web Service Development: Building and deploying containerized web services.
Prompt Engineering: "Did a lot of prompting to make sure final report has Reddit sources," "trigger prompt generation workflow," "Changed 03-mini reasoningEffort setting."
Workflow Automation & Integration:
Triggering and integrating with no-code platforms/workflows (specifically mentioning "n8n workflows," "reddit workflows," "noCode workflow," "NoCode Prompt Generation workflow," "Reddit Insights Enqueuer and Output Writer").
Implementing logic for status checking and sequencing of automated tasks.
Queueing Systems: Designing and implementing a task queueing system with workers to process tasks sequentially (e.g., "queueing system feature," "worker pulling tasks from the queue").
Task Scheduling: Implementing features to schedule tasks (e.g., "schedule a new one for 7days later").
Data Processing & Manipulation: "Removing unwanted data, empty strings, null values" from SoV Report data.
PDF Generation: Researching and implementing HTML/Markdown to PDF generation (mentioning "apitemplate.io").
Databases:

MongoDB Atlas: Explicitly chosen and used as the database service.
MongoDB (General):
Schema Design/Data Modeling: Designing initial MongoDB schemas and iterating based on feedback.
Database setup and seeding with test data.
Creating and managing collections (tasks, users, permissions, product research, report chunks, etc.).
Database Integration: Connecting the API to the database for storing and retrieving data.
Deployment & DevOps:

Cloud Platforms:
Vercel: Initial deployment platform for deepResearcher.
Render.com: Switched to for hosting deepResearcher as a containerized web service and also for the Snapshots API service.
CI/CD:
Planning and researching CI/CD pipelines for easy deployment from GitHub.
Integrating tests into the CI/CD pipeline.
Production Environment Management: Deploying to production, fixing bugs in production, pushing updates.
Containerization: Implied by "containerized web service" on Render.com.
Testing:

API Testing: General testing of API endpoints, transferring API Spec to Postman for faster development and testing, implementing example responses.
Unit Testing: Implementing general unit tests, aiming for decent code test coverage, sprinkling unit tests.
Integration Testing: Implied by testing the "whole workflow end to end."
Debugging: Significant time spent on debugging issues in development and production environments (e.g., "integration bugs," "fixed some bugs," "debugging with Michał," "Applying fixes/debugging to SoV Report data").
Tools & Platforms:

Postman: Used for API specification, development, and testing.
Git/GitHub: Implied by "deployment from github."
Scira.app: Identified as an open-source search engine with a good UI.
n8n: No-code workflow automation tool.
Sentry: Used for error handling (SDK integration) and uptime monitoring.
APImonitor / APItemplate.io: Researched and used for PDF generation.
Slack: Used for team communication and potentially for API error notifications.
Firebase: Implied for user authentication ("All firebase users with company emails have access").
Software Development Practices & Soft Skills:

Agile/Iterative Development: Iterating on API specs and features based on feedback, daily updates, and "Next Steps" planning.
Collaboration: Working closely with team members (Michał, Bartosz, Adam, David) for feedback, discussions, and requirements gathering.
Communication: Providing regular and detailed daily updates, participating in meetings.
Problem Solving: Identifying and fixing bugs, finding solutions for deployment issues, researching and evaluating tools/techniques.
Requirements Gathering & Analysis: Discussing initial requirements and acceptance criteria.
System Design: Designing API services, database schemas, and workflow integrations.
Research & Evaluation: Researching open-source tools, deployment options, API user management techniques, PDF generation libraries, monitoring systems.
Documentation: Creating API documentation.
Code Refactoring: "Refactoring, removing unused code/files and comments across the codebase."
Security:
Implementing user authentication (bearer token, hashed API keys).
Managing user roles and permissions for folder/product access.
Restricting access for users outside company domains.
Skill Stack Summary:

Here's a more condensed "Skill Stack" based on the above:

Programming Languages & Backend:

Python
API Design & Development (RESTful principles implied)
Web Service Development
Workflow Automation & Integration (n8n, Custom Logic)
Queueing Systems & Task Scheduling
Prompt Engineering
Databases:

MongoDB (Atlas, Schema Design, CRUD, Aggregation implied)
DevOps & Deployment:

Render.com, Vercel
CI/CD (GitHub Actions or similar implied)
Containerization (Docker implied)
Testing:

API Testing (Postman)
Unit Testing
Debugging
Tools & Platforms:

Postman
Git/GitHub
Sentry (Error Tracking, Monitoring)
APItemplate.io (PDF Generation)
Firebase (Authentication)
Methodologies & Soft Skills:

Agile/Iterative Development
Collaboration & Teamwork
Strong Communication (Written & Verbal)
Problem-Solving & Analytical Thinking
System Design
Technical Research & Evaluation
API Documentation
Security Best Practices (Authentication, Authorization)