# Java Development Standards

## Code Style & Formatting
- Follow Java naming conventions:
  - Classes: PascalCase (e.g., `QueryExecutor`, `PPLParser`)
  - Methods/Variables: camelCase (e.g., `executeQuery`, `parseExpression`)
  - Constants: UPPER_SNAKE_CASE (e.g., `MAX_RETRY_COUNT`)
  - Packages: lowercase with dots (e.g., `org.opensearch.sql.ppl`)
- Use proper JavaDoc comments for public methods and classes
- Maintain consistent indentation (4 spaces, no tabs)
- Keep line length under 120 characters
- Use meaningful variable and method names that express intent

## Documentation Requirements
- All public classes must have JavaDoc with class purpose
- All public methods must have JavaDoc with:
  - Brief description of what the method does
  - @param descriptions for all parameters
  - @return description if method returns a value
  - @throws for any checked exceptions
- Complex algorithms should have inline comments explaining the logic
- Update relevant documentation when modifying existing functionality

## Error Handling
- Use specific exception types rather than generic Exception
- Always provide meaningful error messages
- Log errors at appropriate levels (ERROR, WARN, INFO, DEBUG)
- Handle null values explicitly - prefer Optional<T> for nullable returns
- Use try-with-resources for resource management

## Code Organization
- Keep classes focused on single responsibility
- Prefer composition over inheritance
- Use interfaces to define contracts
- Group related functionality into packages
- Separate concerns: parsing, execution, storage, etc.

## Performance Considerations
- Avoid creating unnecessary objects in loops
- Use StringBuilder for string concatenation in loops
- Consider lazy initialization for expensive operations
- Profile code when performance is critical
- Use appropriate data structures for the use case

## Security Guidelines
- Validate all inputs, especially user-provided queries
- Sanitize data before logging to prevent log injection
- Use parameterized queries to prevent SQL injection
- Be cautious with reflection and dynamic class loading
- Follow principle of least privilege for permissions
