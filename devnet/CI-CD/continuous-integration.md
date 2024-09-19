# Continuous Integration:
## Overview:
### Software developers integrate code into a shared repository several times a day.
- All teams use central source control repository instead of separate branches.
- They know how their code works best, and how it integrates.
### Build:
- Compiled regularly, even every time someone checks in code.
- Compiled on dedicated server. Centralized and controllable and provides results to devs.
### Automated tests:
- Runs against compiled code or temporary local deployment of code.
- Security, functionality, performance.
### Principles:
- Code lives in a single place
- Everyone commits to main multiple times a day
- Automate build/test process
    1. Make it fast for quick feedback.
    2. Run every time code is checked in.
    3. Integrated automated test
- Everyone can see results to make improvements
### Benefits:
1. Integration takes less effort
2. Issues will come up more early
3. Automation means less human error/issues
4. Process is more visible
5. Teams are no longer in silos
6. Short feedback loops = better response to customer needs
7. Code is delivered more often
8. With CI, software is:
    - Better
    - Faster
    - Cheaper
    - Flexible

## Implementation
1. Get to a single source code repository
    - Establish a strong branching strategy - everything merges back to main lines
    - Merge to a single repo
    - Double down on collaboration
2. Create Automated Build Process
    - Use a dedicated Server
    - Install build engine
    - Create build definitions - scripts/automation is a code artifact belongs in repo
3. Create Automated Test Process
    - Run static test with the build
    - (Optional) deploy the code to run live tests
    - Advice: run test in parallel