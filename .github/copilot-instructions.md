# GitHub Copilot Instructions

## Project Overview

This is the "pages" repository - a project designed for web pages and related content. This file provides guidance to GitHub Copilot and developers working on this project.

## General Principles

### Ask Before Assuming
- **Always ask clarifying questions** before making significant architectural decisions or implementing complex features
- When requirements are ambiguous, seek clarification rather than making assumptions
- Confirm understanding of user stories and acceptance criteria before implementation

### Code Quality Standards
- Write clean, readable, and maintainable code
- Follow the principle of least surprise - code should do what it appears to do
- Keep functions small and focused on a single responsibility
- Use descriptive variable and function names that clearly express intent
- Avoid premature optimization - prioritize clarity first, optimize only when necessary

## Coding Standards

### General Style Guidelines
- Use consistent indentation (2 spaces for JavaScript/TypeScript/HTML/CSS, 4 spaces for Python)
- Keep line length reasonable (aim for 80-100 characters, max 120)
- Use meaningful comments to explain "why", not "what"
- Remove commented-out code before committing
- Ensure all files end with a newline character

### Naming Conventions
- Use `camelCase` for JavaScript/TypeScript variables and functions
- Use `PascalCase` for classes and components
- Use `UPPER_SNAKE_CASE` for constants
- Use descriptive names that convey purpose and context
- Avoid abbreviations unless they are widely understood

### Error Handling
- Always handle errors gracefully and provide meaningful error messages
- Use try-catch blocks for operations that may fail
- Log errors appropriately for debugging
- Never expose sensitive information in error messages

## Testing Requirements

### Test Coverage
- Write tests for all new features and bug fixes
- Aim for high test coverage, but focus on meaningful tests over percentage targets
- Include unit tests for individual functions and modules
- Add integration tests for critical user flows
- Test edge cases and error conditions

### Test Quality
- Tests should be deterministic and not depend on external state
- Use descriptive test names that explain what is being tested
- Follow the Arrange-Act-Assert (AAA) pattern
- Keep tests simple and focused on one thing
- Mock external dependencies appropriately

### Running Tests
- Ensure all tests pass before submitting a pull request
- Run tests locally before pushing changes
- Fix any failing tests immediately - don't commit broken tests

## Documentation Expectations

### Code Documentation
- Document all public APIs, functions, and classes
- Include JSDoc/docstring comments for complex functions
- Document function parameters, return values, and exceptions
- Keep documentation up-to-date with code changes

### README and Guides
- Maintain an up-to-date README.md with project overview and setup instructions
- Document installation steps, dependencies, and prerequisites
- Include usage examples and common workflows
- Document configuration options and environment variables

### Inline Comments
- Use comments to explain complex logic or non-obvious decisions
- Explain the reasoning behind workarounds or unusual patterns
- Update comments when code changes
- Remove outdated or misleading comments

## Architecture Patterns

### Project Structure
- Organize files logically by feature or functionality
- Keep related files together
- Use clear directory names that indicate purpose
- Separate concerns (presentation, business logic, data access)

### Design Patterns
- Apply established design patterns where appropriate
- Favor composition over inheritance
- Use dependency injection for better testability
- Keep components loosely coupled and highly cohesive

### Performance Considerations
- Be mindful of performance implications in critical paths
- Optimize database queries and API calls
- Implement caching where appropriate
- Consider lazy loading for large resources

## Git and Version Control

### Commit Messages
- Write clear, concise commit messages in imperative mood
- Start with a short summary line (50 characters or less)
- Add detailed description if needed, separated by blank line
- Reference issue numbers where applicable

### Pull Requests
- Create small, focused pull requests that address a single concern
- Write descriptive PR titles and descriptions
- Include testing steps and screenshots for UI changes
- Respond to review comments promptly and professionally

### Branch Management
- Create feature branches from the main branch
- Use descriptive branch names (e.g., `feature/add-navigation`, `fix/login-bug`)
- Keep branches up-to-date with the main branch
- Delete branches after merging

## Security Best Practices

### General Security
- Never commit secrets, API keys, or passwords
- Use environment variables for sensitive configuration
- Sanitize user input to prevent injection attacks
- Validate and sanitize data on both client and server
- Keep dependencies up-to-date to patch security vulnerabilities

### Authentication and Authorization
- Implement proper authentication mechanisms
- Use secure password hashing (bcrypt, Argon2)
- Implement proper session management
- Apply principle of least privilege for permissions

## Collaboration Guidelines

### Code Reviews
- Review code thoroughly and provide constructive feedback
- Focus on code quality, maintainability, and correctness
- Be respectful and professional in all communications
- Explain your suggestions and reasoning

### Communication
- Be clear and concise in written communication
- Use appropriate channels for different types of communication
- Respond to questions and requests in a timely manner
- Document decisions and important discussions

## Accessibility

- Follow WCAG guidelines for web content
- Ensure proper semantic HTML structure
- Include appropriate ARIA labels and roles
- Test with screen readers and keyboard navigation
- Maintain sufficient color contrast ratios

## Performance and Optimization

- Minimize bundle sizes and optimize assets
- Implement code splitting where beneficial
- Optimize images and media files
- Use appropriate caching strategies
- Monitor and profile performance metrics

## Continuous Improvement

- Stay updated with best practices and new technologies
- Refactor code when you see opportunities for improvement
- Share knowledge and learnings with the team
- Provide feedback on processes and workflows
- Learn from mistakes and adapt accordingly

---

**Remember**: These guidelines are meant to help maintain code quality and consistency. When in doubt, ask questions and seek feedback from the team. Quality and clarity should always take precedence over speed.
