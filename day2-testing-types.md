Topics :- Smoke, Sanity, regression, functional

1Q) What is functional Testing? Explain its primary Objective.
Ans: Functional Testing is a type of software testing that verifies whether an application behaves acording to the Specified requirements Or business logic.
Primary Objective:
1) Validate what the system does
ii) Ensure Each feature works requirements as expected based on requirements
Example:
1) Login functionality -> Valid Credentials should allow access
2) invalid credentials -> error message should be displayed


2Q) What is the difference between Smoke Testing and Sanity Testing?
Ans:Smoke vs Sanity Testing
Aspect                Smoke testing                            Sanity Terting
purpose               check basic stability of build           validate Specific functionality after changes
Scope                 Broad (covers major features)            Narrow (focused area)
When                  After new build deployment               After bug fix or minor change
Depth                 Shallow                                  Deep
Example                App launches, login works               Check only payment module after fix

Key idea:
Smoke = Build is testable
Sanity = Fix is working correctly


3Q) What is Regression Testing? Why it is importany in automation?
Ans: Regression Testing ensures that new changes, Bug fixes, or enhancements do not break existing functionality
Importance in Automation
1) Repetitive -> ideal for automation
2) Saves time vs manual execution
3) Ensures stability across releases
Example:
Fix in payment module -> Verify login, cart, checkout still work

4Q) When should you perform Smoke, sanity and regression testing in  a typical SDLC cycle?
Ans: Smoke Testing:
1) Immediately after a new build is deployed
2) Before detailed testing starts
Sanity Testing:
1) After bug Fixes or Small Changes
2) To verify Specific Functionality
Regression Testing:
1) After Major Changes releases, Or multiple fixes
2) Before production releases

5Q) In an automation frameworks, how would you decide which test case belong to:
->Smoke  suite
->Sanity Suite
-> Regression Suite
Explain With reasoning (not just definations)
Ans: Smoke Suite:
1) Critical functionaliteis only
2) Should run quickly (5-15mins)
Examples:
1) App launch
2) Login
3) Basic Navigation

Sanity Suite
1) Test Cases related to recent changes
2) Focused and limited
Examples:
=> login, Search, Cart, Checkouts, Logout etc
Decision Criteria 
1) Business Critically
2) Frequency of use
3) Risk of failure

6Q) A new build is deployed for an e- commerce website. Login is working , but the " add to cart" button is failing
1) What type of testing do you perform first?
2) What will be your next steps?
Ans: First=> Smoke Testing
=> Verify if build is stable ( login works, navigation works)
next steps:
1) identify if issue is isolated or widespread
2) Perform Functional Testing on cart module
3) Log defect with Proper details
4) After fix => Perform Sanity Testing
5) Later => Include in regression Testing

7Q) A developer fixed a bug in the payment module 
1) which type of testing is most suitable?
2) Do you need to run the full regression suite? why or why not?
Ans: Most Suitable => Sanity Testing
Reasons:
1) Only one module Changed 
2) Need to validate fix Quickly
Full Regression?
1) Not Immediately required
2) But Should be run before release to ensure no side effects.


8Q) Your regression suite has 2000 test cases, and execution takes 8 hours.
1) How will you optimize execution time?
2) which test will you prioritize and why?
Ans: Strategies:
1) Test case Prioritization 
=> Run high - risk and critical test first
2) Parallel Execution
=> USe seleninum Grid/ Cloud tools
3) Tagging Test
=> Smoke/Sanity/ Regression tags
4) Remove Redundant Test
=> Avoid duplicate coverages
5) CI/CD Integration
=> Run tests automatically on builds
Prioritize:
1) Business- Critical flows (login, PAyments)
2) Frequently used features
3) Previously failed areas

9Q) You have automated smoke test, But they are failing frequently even though the application is stable
1) What could be the possible reasons?
2) how would you fix this issue?
Ans: Possible Reasons:
1) Unstable test Scripts(poor locators)
2) Environment issues
3) Test data Problems
4) Timing issues (synchronization)
5) Application dependency failures
Fix: 
1) Use explicit waits instead of hard waits
2) Improve locator startegies ( avoid xpath dependency)
3) Stabilize test data 
4) fix environment issues
5) Add proper error handling and logging


10Q) If you join a company as a fresher automation Tester and they already have:
=> 500+ automated test cases
=> No proper categorization (Smoke/ sanity/Regression Missing)
How will you organize and restructure the test suite professionally?
Ans:  Step -by- step Approach:
1) Analyze existing 500+ test cases
=> understand coverage
2) categorize based on: 
=> critically 
=> frequency
=> Risk
3)  Create tags:
=> Smoke
=> Sanity
=> Regression
4) Build Suites:
=> Smoke-> 20- 30 critical test
=> Sanity -> Module - Based tests
=> Regression -> Full coverage.
5) Refactor Automation Framework:
=> USe tagging (TestNG/ Py Test groups)
6) Integrate with CI/CD
=> Smoke -> Every build
=> Regression -> Nightly/ Pre-release.








