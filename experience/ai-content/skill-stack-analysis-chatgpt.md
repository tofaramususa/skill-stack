# Tofara Mususa - Engineering Skill Stack

This document outlines the comprehensive technical skill stack derived from professional engineering updates and daily development work. It focuses on technologies, tools, and techniques used in backend development, system architecture, DevOps, monitoring, and integration with no-code platforms.

---

## Backend Engineering

### API Design & Development

* RESTful API design using **Postman** collections for spec definition and collaboration
* Endpoint design for:

  * Report generation (Reddit Reports, Snapshots)
  * Task scheduling and queueing systems
  * Product and folder management
* Versioning and documentation through deployed Swagger UI
* Status and health check endpoints for monitoring

### Data Modeling & Database Management

* **MongoDB Atlas**:

  * Schema design and optimization for multiple collections (e.g., tasks, snapshots, user permissions)
  * Efficient indexing strategies for time-triggered events (e.g., weekly snapshot generation)
  * CRUD operation implementation across all models

### Queueing and Scheduling Systems

* Custom queueing implementation:

  * Task pulling workers executed hourly
  * Status tracking for tasks: pending → running → success
* Scheduling feature:

  * Post-snapshot task scheduling (e.g., new snapshot after 7 days)
  * Dynamic task queue modification via API

### Workflow Integration (No-Code Platforms)

* Integration with **n8n** workflows to:

  * Trigger prompt generation
  * Scrape Share of Voice (SoV) data
  * Initiate Reddit data ingestion and insights generation
* Use of polling mechanisms to ensure completion before proceeding to next step

### Testing & Error Handling

* Unit tests sprinkled across services using Python and Node.js testing tools
* Error handling strategies:

  * Graceful fallbacks for external service failures (e.g., Sentry SDK crashes)
  * Debugging complex workflows and handling asynchronous errors

---

## Infrastructure & DevOps

### Deployment & Hosting

* **Vercel**:

  * Rapid frontend/backend deployment for MVP testing
  * Debugged integration mismatches between dev and production

* **Render.com**:

  * Switched to containerized services for unrestricted compute time
  * Hosted production APIs for Snapshots, Reddit Reports

### CI/CD Pipeline

* GitHub → Render automatic deployments
* Pre-deployment hooks:

  * Integrated unit tests
  * Postman collection tests
* Planning phase for full CI/CD automation with secrets management

### Monitoring & Observability

* **Sentry**:

  * Integrated uptime monitoring via `/healthcheck` endpoint
  * Error capturing from all environments
* **Slack Integration** (planned):

  * Real-time error alerts pushed to Slack channels

---

## Security & Access Management

### Authentication & Authorization

* **Firebase Auth**:

  * Bearer token protection across all API endpoints
  * Role-based access control: admin, user, restricted user
* **Permissions System**:

  * Per-folder/product access restrictions
  * Master key usage for admin permission assignments

### API Security

* Hashed API keys stored in MongoDB
* Token validation middleware to protect business logic endpoints

---

## Reporting & Document Generation

### Report Generation Pipelines

* Snapshot pipeline flow:

  * Triggers prompt generation → executes scrapers → stores raw data
  * Generates reports in chunks, then aggregates into final document
* Product research integration:

  * Initial research + prompts stored and reused
  * Journey stage metadata tagging

### PDF Generation

* **APITemplate.io** integration:

  * Markdown → HTML → PDF report creation
  * Generated directly through backend API endpoint
  * Return PDF to frontend via `/pdf` endpoint
* Experimentation with alternative Python packages for PDF rendering

---

## Tooling & Platforms

### Platforms Used

* **MongoDB Atlas** - cloud database
* **Render.com** - container-based app hosting
* **Vercel** - frontend/backend hosting
* **Firebase Auth** - authentication service
* **n8n** - no-code workflow automation
* **APITemplate.io** - dynamic PDF generation

### Developer Tools

* **Postman** - API design and example response testing
* **Sentry** - error tracking and uptime monitoring
* **Slack** - notification integration for workflow observability
* **GitHub** - version control and CI/CD

---

## Engineering Techniques & Practices

### Engineering Practices

* Agile development through daily updates and short feedback loops
* Test-driven improvements and production-first mindset
* Emphasis on developer experience and deployment velocity

### Architectural Principles

* API-first design: all features exposed through REST endpoints
* Modularization of workflows: separation of concerns (e.g., raw data vs. insights)
* Event-driven processing: status checks to trigger downstream logic

---

*This skill stack reflects applied, real-world engineering in a fast-paced team environment with strong product integration, automation, and backend expertise.*
