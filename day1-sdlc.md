Topic: SDLC, STLC, role of a tester

1Q) What is Software Development life cycle and what are its main phases?
Ans: Software development life cycle is a structured process Used to design, develop, test and deliver software efficiently.
Main phases:
1. Requirement Gathering and Analysis
2. Design (HLD & LLD)
3. Development (coding)
4. Testing
5. Deployment
6.Maintenance

2Q)Explain Software Testing Life cycle. how is it different from SDLC?
Ans: Software Testing Life cycle is a Sequence of  testing activities performed to Ensure software Quality.
phases:
1. Requirement Analysis.
2. Test planning
3. Test Case Design
4. Test environment setup
5. Test execution
6. Test closure
Difference:
SDLC focuses on building the product
STLC focuses on validating the product
STLC is a Subject of SDLC

3Q) At which phases of SDLC is a tester activity involve and what are  their responsibilities in each phase? 
Ans:  Tester is involved throught the SDLC, not just testing phase
⇒ Requirement phase:
Review requirements, identity gaps, Create RTM
⇒ Design phase: 
understand architecture, prepare tert strategy
⇒ Development phase:
Create test cases, prepare data
⇒ Testing phase:
Execute test cases log detects
⇒ Deployment phase:
perform smoke / Sanity testing
⇒ Maintenance phase:
Regression testing for Updates

4Q) What is the difference beticeen Verification and Validation? Give practical Examples.
Ans:⇒ Verification "Are we building the product right?" (static testing: reviews, walkthroughs)
    ⇒Validation "Are we building the Light product?"
    (Dynamic testing: Execution)
Example:
checking requirement document > Verification
Running text case on application  > Validation.

5Q). Explain how STLC aligns with SDLC in a real project. Why is this alignment important?
Ans: Each SDLC phase has a corresponding terting activity.
Requirement: Test Requirement Analysis
Design: Test planning
Development: test Case creation
Testing: Test Execution
Deployment: UAT / Release. Testing
Importance
1.early defect detection
2.Reduced cost
3.Better poroduct Quality

6Q) You are working on a project where requirementes are undear and frequently changing.  How wil you handle testing in such a situation?
Ans: Approach
1.follow agile, mindset
2.clarify requirements with stakeholders
3.Write flexible & modular test cases.
4.prioritize critical test scenarios
5.Update RTM regularly

7Q) During testing, you find a critical defect just before release. What steps will you take as a tester?
Ans: steps!
1.Log defect with highly severity & prority
2. unform stakeholders immediately
3. Provide clear evidence (logs, screenshots)
4. Suggest  blocking release if imapcts is high
5. Retest after fix+ run regression.

8Q). Your developer Says. This  bug is not reproducible How will you respond and proceed!
Ans: Approach:
1. Re-check steps and data
2. Record video/screenshots.
3.→verify Environment differences
4.provide logs/ test data
5. Try multiple times

9Q). You executed a test test case yesterday, and it passed Today, the Same test case is failing without any code change.  
What could be the possible reasons, and how will you investigate?
Ans: possible Reasons
1.Environment issue
2.Test data changed
3.Dependency Service failure
4.Configuration changes
5.Timing issues/ flaky test
Investigation steps:
1.compara logs (yesterday vs today)
2.check Environment and data
3.Re-run test
4.Validate build version

10) As a tester, how do you ensure quality a project - not Just "testing"? 
Ans: A good tester Ensures Quality by:
1.Involving Early in SDLC
2.Writing effective text cases
3.practicing risk based testing
4.Automating repetitive test
5.communicating with developer & business teams
6.preventing defects, not just finding them.

