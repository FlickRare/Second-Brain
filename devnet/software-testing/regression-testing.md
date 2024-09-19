# Regression
Main idea: when adding a new feature to an application, test the functionaliy preexisting features.
### When to perform regression testing:
- new functionalities are added
- Change requirement (when removing functionality
- Defect (bug) fix
- Run test on bug fix
- Performance issue it fixed
- Environment change
- Underlying systems (ex: db, OS)
- Patch fix
### Types of regression testing
- Unit testing: when code is changed tester (usually dev) re-runs all previously passed tests in isolation.
- Progressive testing: use when software specifications and test cases are changed.
- Selective testing: Perform only unit tests that cover changed code.
- Retest-all testing: Rerun all tests. Runs avoidable tests and is costly when only making small changes.
- Complete testing: Useful when multiple changes have been done in existing code. Good for finding unexpected bugs. Used for more critical functionalities.
### Testing order:
1. Unit-level regression tests
2. Integrate with the currrent build
3. Smoke test to check the updated build
4. Perform Sanity testing on the new feature/fix
5. Integration testing with other systems
6. Schedule regression tests
### Select test cases which:
- Have frequent defects
- Verify core functionality
- Test complex problems
- Verify integration
- Cover where changes have been made
- Frequently fail
- Boundary value
### Methods:
- Re-testing - full execution of all tests is re-accomplished
- Selective tests - limited number of test chosen against changes
- Prioritization - prioritizes especially important cases
- Hybrid - combines selective and prioritization
### Example regression test plan:
|     Terminology         	|     What it is                                                  	|     Example                               	|
|-------------------------	|-----------------------------------------------------------------	|-------------------------------------------	|
|     Test   Objective    	|     What   you are planning to do                               	|     Check   functionality of a feature    	|
|     Test   Object       	|     Components   to be tested                                   	|     Sort   Feature                        	|
|     Test   Item         	|     Subset   of test object                                     	|     Price:   High to Low, Low to high     	|
|     Test   Condition    	|     Subset   of Item                                            	|     Sorting   by Price: High to Low       	|
|     Test   Case         	|     Parameters:   test data, preconditions, expected results    	|                                           	|
|     Test   Suite        	|     Set of   test cases                                         	|                                           	|

### Traceability:
- The ability to connect requirements to other artifacts — such as different types of software tests or bugs. It's used to track requirements — and prove that requirements have been fulfilled.
- Requirements Traceability Matrix:
    - Demonstrates the relationship between requirements and other artifacts.
    - It's used to prove that requirements have been fulfilled.
    - And it typically documents requirements, tests, test results, and issues.
- Bidirectional Traceability: 
    - Trace forward - from requirement to test case
    - Backward - from test case to requirement
- Benefits: passing an applicable test proves the corresponding requirement has been achieved.
    - Meet goals - keeps team on target with original requirements
    - Run the right test - clear documentation helps choose correct test
    - Making decisions - understand how product design will be impacted by requirements
    - Managing projects - gauge progression and control scope
### Challenges:
- Time consuming and expensive
    - Considered a drain on resources - why test something that we already know works.
    - Implement intelligent method for executing test within time and budget limits.
- Complex and challenging
    - As project expands, devs are overwhelmed by growing pool of test cases
    - Monitor test suites, prune obsolete test, simplify when possible
- Difficult to communicate business value:
    - Most non-technical leaders want to see project move forward rather than use resources on testing old features.
### Best Practices:
- Maintain testing schedule
    - Don't let it fall onto the back burner
- Use a test management tool
    - Streamline tracking process
- Break down and categorize tests
    - Divide into smaller more approachable chunks
- Consider customer risk
    - Keep track of effects of tests on customers
- Evaluate test prioritization
    Avoid unnecessary tests