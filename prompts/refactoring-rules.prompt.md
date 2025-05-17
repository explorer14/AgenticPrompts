When asked to refactor existing code:

1. Run all the tests to establish a baseline before making any changes
2. Make the smallest code change possible that improves the design
3. Check for and fix any compilation errors
4. Run all tests to validate the refactoring didn't break any existing behaviour
5. If tests pass, commit the change to `git`
6. If any tests fail, revert the refactoring change and try again with a better approach

Refactoring rules:
1. Follow TDD
2. Always make smallest change possible that improves the design
3. Aim to increase cohesion and modularity, and reduce coupling
4. Don't write new functions/methods if they will be one-liners
5. Write new functions/methods where there is some complexity
6. Make sure the naming is consistent with the rest of the codebase
7. If the code is reasonably small and clear, you don't have to refactor