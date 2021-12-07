# Backend Engineer Coding Challenge

> This repository contains the coding challenge for backend engineers.

**Note:** Please don't fork this repository, create a pull request against it, or use GuardRails in the repo name. Otherwise other candidates may take inspiration from it. Once the coding challenge is completed, you can submit it via this [Google form](https://forms.gle/i5nZWZKoUnTWj3td9).

## Description

Build a simple code scanning application that detects sensitive keywords in public git repos.
The application must fulfil the following requirements:
- A user can CRUD repositories. A repository contains a name and a link to the repo.
- A user can trigger a scan against a repository.
- A user can view the Security Scan Result ("Result") List

How to do a scan:
- Just keep it simple by iterating the words on the codebase to detect SECRET_KEY findings.
- SECRET_KEY start with prefix public_key || private_key.

The Result entity should have the following properties and be stored in a database of your choice:
- Id: any type of unique id
- Status: "Queued" | "In Progress" | "Success" | "Failure"
- RepositoryName: string
- RepositoryUrl: string
- Findings: JSONB, see [example](example-findings.json)
- QueuedAt: timestamp
- ScanningAt: timestamp
- FinishedAt: timestamp

Wherever you'd have to add something that requires product subscriptions or significant extra time, just mention it in your documentation.

**What we want to see:**
- Project Structure: Clear organization and structure of folders, code and functionality.
- Clean Code: Code Consistency, use of linters, formatting, error handling, and anything else that shows your skills. Simple is better than complex.
- Stack Knowledge: Proper use of Golang and selected frameworks/libraries.
- Implementation: The implementation has to work according to the specs.
- Unit Tests: Covering the core functionality with unit tests (positive and negative test-cases).
- Proper Documentation: 
    - A High-Level Design for the components/infrastructure if any.
    - Describe how you came up with the solution and what makes it a good one for the use-case.
    - Describe what the project is doing, what has been used, how to configure it, how to start it, test it etc.

**Bonus points for:**
- SQL schema
- API documentation
- Containerized app
- Use of appropriate design patterns
- Microservice Architecture
- Any extra feature (just write it in your documentation)

**Things you don't have to worry about:**

- Authentication/Authorization
- CI configuration / Deployment
- APM
- Authentication / Authorization / Auditing
