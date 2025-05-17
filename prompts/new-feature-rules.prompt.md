When asked to write a new feature:

1. Write a test that fails the expected behaviour
2. Write minimal code that passes the test
3. Refactor code if necessary. Follow the [refactoring rules](refactoring-rules.prompt.md) for this
4. Run the tests to validate the refactoring. If any test fails, revert the changes upto this point, and try with a better approach
5. If all tests pass, commit the change to git by running `git cac` followed by a descriptive but brief commit message.