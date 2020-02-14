# Back-end Engineer Challenge

> This repository contains the challenge for back-end engineers.

**Note:** Please don't fork this repository, or create a pull request against it. Otherwise other applicants may take inspiration from it. Once the coding challenge is completed, you can submit it via this [Google form](https://forms.gle/f2hekWPJqee6htH28).

## Back-end Exercise

Create the project in a dedicated repository with meaningful commit messages. Use Node.js and any framework, if you want to use one.

Implement a **RESTful API** to **CRUD** a Security Scan Result (“Result”). The Result entity should have the following properties:

- Id: any type of unique id
- Status: "Queued" | "In Progress" | "Success" | "Failure"
- RepositoryName: string
- Findings: JSONB, see [example](example-findings.json)
- QueuedAt: timestamp
- ScanningAt: timestamp
- FinishedAt: timestamp

The Result entity should be stored in a database (of your choice). Wherever you’d have to add something that you feel requires product subscriptions or significant extra time, just mention it in your documentation.

**What we want to see:**

- Proper Documentation: Describe what the project is doing, what has been used, how to configure it, how to start it, test it etc.
- Project Structure: Clear organization and structure of folders, code and functionality.
- Clean Code: Code Consistency, use of linters, formatting, error handling, simple and performant solution to the challenge.
- Stack Knowledge: Proper use of node.js, any used frameworks and their latest features.
- Implementation: The implementation has to work according to the specs.
- Unit Tests: Covering the core functionality with unit tests.

**Bonus points for:**

- SQL schema: Using a relational database that has a proper schema
- API documentation: Using e.g OpenApi specs

**Things you don’t have to worry about:**

- CI configuration / Deployment
- APM
- Authentication / Authorization / Auditing
