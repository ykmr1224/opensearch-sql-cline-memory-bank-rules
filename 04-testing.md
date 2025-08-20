# Testing Requirements

## Test Coverage Standards
- Unit tests required for all new business logic
- Integration tests for end-to-end scenarios
- Parser tests for grammar changes
- Calcite integration tests for query planning
- Performance tests for critical paths

## Test Organization
- Follow existing test structure in each module
- Unit tests in `src/test/java` directory
- Integration tests in `integ-test/` module
- Test utilities and base classes in appropriate packages

## Test Execution Commands
- Run all tests: `./gradlew test`
- Module-specific tests: `./gradlew :core:test`, `./gradlew :ppl:test`
- Integration tests: `./gradlew :integ-test:integTest`
- Build and test: `./gradlew build`

## PPL Parser Testing
- Test new grammar rules with positive and negative cases
- Verify AST generation for new syntax
- Test error handling for malformed queries
- Include edge cases and boundary conditions

## Function Testing
- Test function implementations in isolation
- Verify SQL and PPL compatibility where applicable
- Test error conditions and edge cases
- Performance testing for complex functions

## Integration Testing
- End-to-end query execution tests
- Cross-module functionality verification
- OpenSearch integration scenarios
- Backward compatibility validation

## Test Data Management
- Use meaningful test data that reflects real-world scenarios
- Clean up test resources after execution
- Avoid dependencies between test cases
- Use parameterized tests for multiple input scenarios

## Continuous Integration
- All tests must pass before merging
- Run integration tests on significant changes
- Monitor test execution time and optimize slow tests
- Maintain test stability and reliability
