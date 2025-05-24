Tools
MongoDB Atlas: Used as the database service for storing data (e.g., product data, prompts, tasks).
Postman: Utilized for creating, testing, and documenting API specifications and endpoints.
Vercel: Initial hosting platform for deploying the deepResearcher application.
Render.com: Hosting platform used for containerized web services, replacing Vercel for better compute time flexibility.
Sentry: Integrated for error handling, monitoring, and uptime health checks (e.g., Sentry Uptime Monitor).
APITemplate.io: Used for generating PDFs from Markdown for Reddit Reports.
Apimonitor: Set up for API health monitoring.
Slack: Explored for integration with the API for real-time error notifications and updates.
n8n: No-code platform used for automating workflows (e.g., prompt generation, Reddit data scraping).
GitHub: Referenced for version control and CI/CD pipeline planning.
Scira.app: Open-source search engine evaluated for its frontend UI for deepResearcher.
Techniques
API Development:
Designed and iterated API specifications (e.g., Snapshots API, Reddit endpoints).
Implemented CRUD operations for various endpoints.
Created Postman collections for testing and documentation.
Added authentication (bearer tokens) and role-based permissions.
Database Management:
Designed MongoDB schemas for products, folders, prompts, tasks, and Share of Voice (SoV) data.
Seeded test data and managed data integrity checks.
Implemented task scheduling and queueing systems in MongoDB.
Backend Development:
Built backend logic for triggering no-code workflows and handling API requests.
Refactored code to remove unused files/comments and improve maintainability.
Added error handling and integrated Sentry for logging.
DevOps:
Deployed applications to Vercel and Render.com, addressing integration bugs.
Planned and researched CI/CD pipelines for automated deployments from GitHub.
Set up health check monitors and explored real-time error notifications via Slack.
Workflow Automation:
Integrated APIs with no-code platforms (e.g., n8n) for automated workflows like prompt generation and report creation.
Developed a queueing system with workers to execute tasks sequentially.
Implemented status-checking mechanisms for workflow completion.
Testing and Quality Assurance:
Wrote unit tests to improve code coverage.
Conducted general testing of API endpoints and workflows to identify and fix bugs.
Tested user access controls and folder permissions.
Data Processing and Reporting:
Developed Share of Voice (SoV) and Reddit Insights reports, integrating Reddit workflow data.
Cleaned data by removing unwanted entries (e.g., empty strings, null values).
Converted Markdown to HTML to PDF for report generation.
User Management:
Researched and implemented API user authentication with hashed API keys and user roles.
Set up permissions for folder and product access based on user roles.
Technologies
MongoDB: NoSQL database used for data storage and schema design.
Node.js: Inferred as the primary backend runtime environment (based on MongoDB, Vercel/Render usage).
Python:
Used for updating packages and experimenting with HTML-to-PDF generation.
Likely used in Reddit workflow logic and report generation.
Markdown: Used for structuring Reddit Reports before conversion to PDF.
REST APIs: Core technology for building and managing Snapshots and deepResearcher endpoints.
Firebase: Used for user authentication (inferred from company email-based access control).
SERP (Search Engine Results Page): Utilized for Reddit workflow data scraping and insights generation.
Reddit Workflows: Custom workflows for scraping and processing Reddit data for reports.
HTML/CSS: Involved in experimenting with HTML-to-PDF conversion for reports