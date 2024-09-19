# Smoke vs Sanity Testing
## Functional vs non-functional testing
- Functional: tests a function of the application to make sure it works under given conditions. 
	- Types of functional tests:
		- Unit (testing)
		- Integration
		- System
		- Interface
		- Smoke
		- Sanity
		- Regression
		- Acceptance
- Non-functional: determine performance, measure/validate/verify quality of the system.
	- Types of non-functional test:
		- Documentation (testing)
		- Installation
		- Performance
		- Reliability
		- Security
### Software build definition:
Otherwise known as code build or integration, process of taking all source code files that make an app and compiling them into build artifacts such as binaries or executables.
### Smoke testing
- What is smoke testing?
	- AKA: Build verification test. Performed directly after software build to test the critical functionalities.
	- Before any other kind of functional testing
	- Goal: reject badly broken software builds early, save time
- How to conduct a smoke test
	- Choose test cases from test suites cover the major functionalities
	- Test main workflow, not going into detail
### Sanity testing
- What is sanity testing?
	- After receiving software build with minor changes to solve bugs or other fixes
	- Determining if the fixes actually work
	- Make sure the dev is in their right mind
	- Conducted on stable builds, happens later on in testing process
	- Could be considered subset of regression testing
		- Regression testing is for new features
		- Sanity testing is for bug fixes or patches
- How to conduct sanity test
## Smoke vs. Sanity:
- Builds:
	- Smoke testing runs on initial builds
	- Sanity testing runs on builds that pass smoke test and many rounds of regression testing.
- Motive:
	- Smoke: core functionalities work
	- Sanity: verify new functionality and bugs are fixed
- Subsets:
	- Smoke testing: subset of regression testing
	- Sanity testing: subset of acceptance testing
- Coverage:
	- Smoke: Shallow and wide - main functionalities
	- Sanity: Narrow and deep - detailed testing of functionality and features
- Performed by:
	- Smoke: Developers and other testers (automated)
	- Sanity: executed manually by testers
