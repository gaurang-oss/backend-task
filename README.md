# MERN CRM Backend Development Guide


---

# Project Overview

The goal is to build a **production-quality MERN backend** that powers an existing React frontend.

The intern should **not think in terms of "making APIs."**

Instead, they should think like a software architect building an actual SaaS product.

The AI coding agent should be responsible for writing code, while the intern focuses on:

* Understanding the architecture
* Reviewing generated code
* Testing features
* Asking the AI to improve implementations
* Keeping the project organized

The prompts below are intentionally **code-agnostic**.

They describe *what* should exist rather than *how* it must be implemented, allowing the coding agent to choose appropriate libraries, patterns, and optimizations.

---

# Final Product

The finished system should include

* React Frontend (already exists)
* Node Backend
* Express API
* MongoDB Database
* Authentication
* Authorization
* Admin Panel
* User Dashboard
* Job Portal
* CRM Features
* File Uploads
* Search
* Filtering
* Audit Logs
* Notifications
* Production-ready architecture

The backend should be modular enough that future developers can easily add new modules.

---

# Learning Philosophy

Never ask the AI:

> Build login.

Instead ask

> Design and build a scalable authentication module suitable for a production CRM.

The AI will usually produce far better architecture.

---

# Project Modules

The CRM should eventually contain

## Authentication

* Signup
* Login
* Logout
* Forgot Password
* Reset Password
* Refresh Tokens
* Email Verification
* JWT
* Session Management

---

## User Management

Users can

* Register
* Login
* Create profile
* Edit profile
* Upload resume
* Upload profile picture
* Add skills
* Add education
* Add work experience
* Add certifications
* Save jobs
* Apply for jobs
* Track applications

---

## Admin Panel

Admins should have complete control.

Admins can

* View users
* Delete users
* Suspend users
* Restore users
* View applications
* Delete applications
* Create jobs
* Edit jobs
* Delete jobs
* Close jobs
* Reopen jobs
* Create categories
* Manage permissions
* View reports
* View statistics
* View logs

---

## Job Portal

Jobs should support

* Title
* Description
* Company
* Salary
* Employment Type
* Remote/Hybrid/Onsite
* Location
* Experience Required
* Skills
* Benefits
* Status
* Deadline
* Recruiter
* Posted Date

Users should be able to

* Search
* Filter
* Apply
* Save
* Share

---

## CRM

The CRM should maintain

* Every user
* Every job
* Every application
* Every login
* Every action
* Every admin action
* Every notification

Everything should be traceable.

---

## Notifications

Support

* Email
* In-app notifications

Examples

Application submitted

Job closed

Password changed

Admin updated profile

---

## Analytics

Dashboard should display

* Users registered
* Jobs posted
* Applications received
* Active jobs
* Closed jobs
* Most popular jobs
* Daily registrations
* Monthly registrations
* Application trends

---

# Development Roadmap

Do not build everything at once.

The AI should complete one module before moving to another.

---

# Prompt 1

## Project Planning

```
You are a senior software architect.

I want to build a production-grade MERN CRM that functions as a complete job portal.

The frontend already exists in React.

Before writing any code, analyze the project and produce:

• Overall architecture
• Folder structure
• Backend modules
• Database collections
• Relationships
• Authentication flow
• Authorization model
• API conventions
• Validation strategy
• Error handling strategy
• Logging strategy
• Configuration management
• Deployment considerations
• Scalability considerations
• Security considerations

Do not generate code yet.

Instead create a complete technical implementation plan similar to what would be prepared before starting a commercial software project.
```

---

### Why this prompt?

A professional developer plans first.

The AI creates a blueprint.

Only after the architecture is reviewed should coding begin.

---

# Prompt 2

## Backend Initialization

```
Using the previously designed architecture, initialize the backend project.

The backend should follow modern Node.js best practices.

Generate the complete project structure with configuration, middleware, environment handling, routing architecture, utilities, shared services, validation strategy, logging foundation, database initialization, and development tooling.

The backend should be modular, maintainable, scalable, and production-ready.

Avoid implementing business features yet.
```

---

### Why?

Never mix architecture with business logic.

---

# Prompt 3

## Authentication Module

```
Design and implement a complete authentication module suitable for a commercial SaaS CRM.

Support:

User registration

Secure login

JWT authentication

Refresh tokens

Password hashing

Email verification

Forgot password

Reset password

Logout

Session management

Role-based authentication

Admin authentication

Input validation

Rate limiting

Security best practices

The module should expose clean APIs and integrate naturally into the overall backend architecture.
```

---

### Why?

Authentication is the foundation.

---

# Prompt 4

## User Module

```
Design a complete user management system.

Users should have professional profiles similar to LinkedIn.

Include personal information, contact information, education, work experience, skills, certifications, resume uploads, profile images, social links, preferences, privacy settings, and account settings.

The module should support profile editing, searching, filtering, validation, and secure ownership rules.

Ensure the design remains extensible for future enhancements.
```

---

# Prompt 5

## Admin Module

```
Design a complete administrative module.

Administrators should have centralized control over the platform.

Include:

User management

Job management

Application management

Role management

Permission management

Platform configuration

Dashboard statistics

Activity logs

Audit logs

Reports

System settings

Notifications

Every administrative action should be traceable and logged.

Design the module to scale as the application grows.
```

---

# Prompt 6

## Job Module

```
Design a professional recruitment system.

Administrators should be able to create, edit, publish, archive, duplicate, close, and reopen job postings.

Jobs should contain comprehensive metadata, searchable fields, filtering capabilities, categorization, tags, application deadlines, recruiter ownership, publication status, and SEO-friendly identifiers where appropriate.

Users should be able to browse, search, filter, save, and apply for jobs.

The system should support future expansion without major architectural changes.
```

---

# Prompt 7

## Application Module

```
Design the job application workflow.

Users should be able to apply to jobs using their profile and uploaded resume.

Applications should maintain lifecycle states such as submitted, under review, shortlisted, rejected, interview scheduled, offered, hired, and withdrawn.

Maintain complete application history and timestamps.

Administrators should be able to review, filter, update, comment on, and manage applications.

Ensure proper ownership validation and secure business rules.
```

---

# Prompt 8

## Dashboard Module

```
Create dashboard APIs for both administrators and users.

Administrator dashboards should expose meaningful business analytics, operational metrics, growth statistics, recent activities, and platform summaries.

User dashboards should summarize profile completion, saved jobs, applications, application statuses, recommendations, and notifications.

Design the APIs to be efficient and scalable.
```

---

# Prompt 9

## Search Module

```
Design a search system across the CRM.

Support searching users, jobs, applications, companies, skills, and other entities.

Include filtering, pagination, sorting, keyword search, advanced search, and efficient querying.

Design the APIs for performance while remaining flexible for future enhancements.
```

---

# Prompt 10

## File Management

```
Design a centralized file management module.

Support uploads for resumes, profile pictures, company logos, and other future assets.

Ensure validation, storage abstraction, access control, metadata management, and cleanup strategies.

The implementation should allow changing storage providers in the future without significant code changes.
```

---

# Prompt 11

## Notifications

```
Design a notification system.

Support in-app notifications and email notifications.

Notifications should be event-driven where appropriate and easily extendable to additional delivery channels such as SMS or push notifications in the future.

Include user notification preferences and administrative announcements.
```

---

# Prompt 12

## Audit Logging

```
Design an audit logging system.

Track all important user and administrator actions.

Logs should include actor, action, timestamp, affected resource, previous state when appropriate, new state, IP information where available, and contextual metadata.

Ensure logs are immutable and suitable for troubleshooting and compliance.
```

---

# Prompt 13

## API Documentation

```
Generate comprehensive API documentation for the entire backend.

Include endpoint descriptions, request formats, response formats, validation requirements, authentication requirements, authorization requirements, error responses, and practical usage examples.

The documentation should remain synchronized with the implemented APIs.
```

---

# Prompt 14

## Frontend Integration Review

```
Analyze the existing React frontend.

Compare it against the implemented backend.

Identify:

Missing pages

Missing forms

Missing API integrations

State management improvements

Authentication flow adjustments

Role-based UI requirements

Validation improvements

Loading states

Error handling

Pagination

Filtering

Search

Accessibility improvements

Responsive behavior

Provide a prioritized implementation plan before making changes.

Then implement only the necessary frontend modifications while preserving the existing design wherever possible.
```

---

# Prompt 15

## Production Readiness Review

```
Perform a complete engineering review of the entire application.

Evaluate:

Architecture

Folder structure

Database design

Security

Authentication

Authorization

Validation

Performance

Scalability

Logging

Testing

API consistency

Error handling

Code organization

Documentation

Developer experience

Deployment readiness

CI/CD readiness

Configuration management

Identify weaknesses, explain why they matter, and improve the implementation where appropriate while maintaining compatibility with the existing system.
```

---

# How to Work with the AI Coding Agent

The intern should follow this workflow for every feature:

1. **Plan first**: Ask the AI to explain the feature, architecture, and tradeoffs before requesting code.
2. **Generate incrementally**: Build one module at a time instead of asking for the entire backend in one prompt.
3. **Review the output**: Read the generated code, understand the folder structure, API design, and database models, then ask follow-up questions about anything unclear.
4. **Test continuously**: Verify each module with API testing tools and the React frontend before moving on.
5. **Refine**: Ask the AI to improve performance, security, readability, or scalability rather than accepting the first implementation.
6. **Integrate carefully**: After backend changes, ask the AI to identify any frontend updates needed, such as new forms, routes, validation, API calls, or state management changes.
7. **Document as you go**: Request updated API documentation and architectural notes whenever a module changes.

---
