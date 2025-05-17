When asked to fix a bug, follow these rules strictly:
1. Write a test first that fails because of the bug and proves the bug exists. Try to write the test at the lowest level module possible to validate the expected behaviour and any return values.
2. Always check for and fix any compilation errors in the test or the code first before attempting to run the new test.
3. Change the code to fix the bug. Only make one incremental change at a time and describe your thinking and reasoning as to why that change might fix the bug.
4. Run the new test you wrote step 1, to validate the changes.
5. If the test passes, commit the changes to git. Otherwise, try to fix the bug again until the test passes.
6. Think of additional test cases that you might want to validate the changes against and make sure they all pass following the steps enumerated above.
7. Finally, as a safety precaution run all the tests to ensure no other regressions were introduced whilst fixing the bug.