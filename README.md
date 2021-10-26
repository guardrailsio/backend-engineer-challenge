# Backend Engineer Coding Challenge

> This repository contains the coding challenge for backend engineers.

**Note:** Please don't fork this repository, create a pull request against it, or use GuardRails in the repo name. Otherwise other candidates may take inspiration from it. Once the coding challenge is completed, you can submit it via this [Google form](https://forms.gle/i5nZWZKoUnTWj3td9).

## Description

Create the project in a dedicated repository with meaningful commit messages. Use Golang and any 3rd party libraries that you want to use.

1. Implement a **RESTful API** to **CRUD** a Security Scan Result (“Result”). The Result entity should have the following properties and be stored in a database of your choice:

- Id: any type of unique id
- Status: "Queued" | "In Progress" | "Success" | "Failure"
- RepositoryName: string
- Findings: JSONB, see [example](example-findings.json)
- QueuedAt: timestamp
- ScanningAt: timestamp
- FinishedAt: timestamp


2. Implement another endpoint that lists all Results and uses pagination.
3. Create unit tests and provide documentation.

Wherever you’d have to add something that requires product subscriptions or significant extra time, just mention it in your documentation.

**What we want to see:**

- Project Structure: Clear organization and structure of folders, code and functionality.
- Clean Code: Code Consistency, use of linters, formatting, error handling, simple and performant solution to the challenge.
- Stack Knowledge: Proper use of Golang.
- Implementation: The implementation has to work according to the specs.
- Unit Tests: Covering the core functionality with unit tests.
- Proper Documentation: Describe what the project is doing, what has been used, how to configure it, how to start it, test it etc.

**Bonus points for:**

- SQL schema: Using a relational database that has a proper schema and indexes
- API documentation: Using e.g OpenApi specs
- Containerized app

**Things you don’t have to worry about:**

- CI configuration / Deployment
- APM
- Authentication / Authorization / Auditing
