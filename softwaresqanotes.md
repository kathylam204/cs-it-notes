# Software Security Testing and QA

## Secure Software Development Life Cycle (SSDLC)
- SDLC is a process for designing, developing, and testing high-quality software.
- Produces software that meets/exceeds customer expectations within time and cost estimates.

## SDLC Models
- Waterfall Model: Linear sequential phases where each phase depends on the deliverables of the previous one.
- Iterative Model: Multiple builds from requirements.
- Agile Model: Interactive and incremental process focused on adaptability and customer satisfaction with rapid delivery.

## Security Standards and Models
- MS Security Development Lifecycle
- NIST 800-64: Security considerations within SDLC, mandatory for US federal agencies.
- OWASP CLASP

## Maturity Models
### Maturity Model: Measures an organization’s ability for continuous improvement.
### Capability Maturity Model (CMM): Evaluates software development process maturity, originally developed by SEI in 1986.
- Five Maturity Levels: Important to know each level and its requirements.
### Testing Maturity Model (TMM): Evaluates and improves testing processes.
- Five Levels: Initial, Phase Definition, Integration, Management and Measurement, Optimization.

## Basic Idea in Software Process
- Activities: Gathering requirements, constructing a functional specification, designing, coding, testing, and maintaining the system.
- Benefits: Repeatability, evaluability, and improvability.

## Software Testing
- Distinct process with unique activities, techniques, and strategies.
- Begins early in the project and continues throughout development.
- Combines manual and automated testing.
- Capability Maturity Model (CMM): Also applied to testing with the Testing Maturity Model (TMM).

## Quality and Improvement
### Quality Models: ISO 9126, CMM, TPI, TMM.
- Verification and Validation:
- Verification: Ensures products meet specified requirements.
### Validation: Ensures products meet intended use.
### Failure, Error, Fault, and Defect: Understanding their definitions is crucial for quality assessment.
### Software Reliability: Probability of failure-free operation; estimated via random testing.

## Testing Processes
- Test Process Improvement (TPI): Evaluates and improves test processes.
- Maturity Levels: Controlled, Efficient, Optimizing.
- Test Cases: Pairs of <input, expected outcome> used to verify software behavior.

## Quality Revolution
- Historical Context: Started in Japan (1940s) by Deming, Juran, and Ishikawa.
- Principles: Continuous improvement, customer focus, and data-driven decisions.
- Total Quality Control (TQC): Emphasizes quality over short-term profits and customer-first approach.
- Statistical Quality Control (SQC): Uses measurement and statistics to manage quality.

## Key Elements of Testing
- Static Analysis: Code review and inspection.
- Dynamic Analysis: Program execution to expose failures.
- Test Oracles: Mechanisms to verify correctness of program outputs.

## The Concept of Complete Testing
### Complete or exhaustive testing means "there are no undisclosed faults at the end of the test phase."
### Complete testing is near impossible for most systems due to:
- The large domain of possible inputs (both valid and invalid).
- Complex design issues that are difficult to test completely.
- The impossibility of creating all possible execution environments.

## The Central Issue in Testing
- Divide the input domain D into D1 and D2.
- Select a subset D1 of D to test program P.
- It is possible that D1 exercises only a part P1 of P.

## Testing Activities
- Identify the objective to be tested.
- Select inputs.
- Compute the expected outcome.
- Set up the execution environment of the program.
- Execute the program.
- Analyze the test results.

## Testing Levels
### Unit Testing: Testing individual program units (e.g., procedures, methods) in isolation.
### Integration Testing: Assembling modules to construct larger subsystems and testing them.
### System Testing: Includes a wide spectrum of testing such as functionality and load testing.
### Acceptance Testing: Ensures the system meets customer's expectations. Includes:
- UAT: System satisfies the contractual acceptance criteria.
- BAT: System will eventually pass the user acceptance test.

## Sources of Information for Test Selection
- Requirement and Functional Specifications.
- Source Code.
- Input and Output Domain.
- Operational Profile.
- Fault Model.
- Error Guessing.
- Fault Seeding.
- Mutation Analysis.

## White-box and Black-box Testing
### White-box Testing (Structural Testing):
- Examines source code with focus on control flow and data flow.
- Applied to individual units of a program.
- Conducted by software developers on the units they write.
### Black-box Testing (Functional Testing):
- Examines the program accessible from outside.
- Applies input to a program and observes the externally visible outcome.
- Applied to both entire programs and individual units.
- Conducted at the external interface level by a separate software quality assurance group.

## Test Planning and Design
### Purpose: To get ready and organized for test execution.
### A test plan provides:
- Framework: Ideas, facts, or circumstances within which tests will be conducted.
- Scope: Domain or extent of test activities.
- Resource details: Effort required, schedule of activities, budget.
### Test cases are designed as combinations of modular test components called test steps, which are combined to create more complex tests.

## Monitoring and Measuring Test Execution
- Metrics for monitoring test execution and defects.
- Test case effectiveness metrics: Measure the "defect revealing ability" of the test suite.
- Test-effort effectiveness metrics: Number of defects found by customers that were not found by test engineers.

## Test Tools and Automation
### Benefits:
- Increased productivity of testers.
- Better coverage of regression testing.
- Reduced durations of testing phases.
- Reduced cost of software maintenance.
- Increased effectiveness of test cases.
### Requirements:
- Well-defined test cases for automation.
- Test tools and infrastructure.
- Experienced test automation professionals.
- vAdequate budget for software tools procurement.

## Test Team Organization and Management
- Hiring and retaining test engineers is challenging.
- Interviews are primary for evaluating applicants; interviewing skills improve with practice.
- Retaining test engineers requires recognizing the importance of testing efforts on par with development efforts.

## Role of Testing
### Software quality assessment:
- Static: Examines the code and reasons over all possible behaviors (e.g., code review, inspection, algorithm analysis).
- Dynamic: Actual program execution to expose possible program failures. Combines both roles for comprehensive testing.

## Test Case
- A simple pair (tuple) of <input, expected outcome>.
- Stateless systems: Outcome depends solely on the current input (e.g., a compiler).
- State-oriented systems: Outcome depends on both the current state of the system and the current input (e.g., an ATM).

## Static Unit Testing
### Inspection: Step-by-step peer group review with predetermined criteria.
### Walkthrough: Author-led team review using pre-defined scenarios.
### Divides and conquers to ensure thoroughness:
- An examiner inspects small parts of the unit in isolation.
- Correctness of all parts implies the correctness of the whole module.

## Static Unit Testing (Code Review) Steps
### Readiness:
- Completeness, Minimal Functionality, Readability, Complexity, Requirements, and design documents.
- Roles: Moderator, Author, Presenter, Record Keeper, Reviewers, Observer.
### Preparation:
- List of Questions, Potential Change Requests (CR), Suggested Improvements.
### Examination:
- Author presents, presenter reads the code, record keeper documents CR, moderator ensures review stays on track.
### Re-work:
- Lists of CRs and improvements; record meeting minutes; author fixes issues.
### Validation:
- Independent validation of CRs.
### Exit:
- Summary report of meeting minutes distributed.
- CR details: Description, priority level, assigned person, deadline.

## Metrics from Code Review
- LOC reviewed per hour.
- CRs per KLOC.
- CRs per hour.
- Total hours spent on the code review process.

## Hierarchy of System Documents
Requirement: High-level marketing or product proposal.
Functional Specification: Software engineering response to the marketing proposal.
High-Level Design: Overall system architecture.
Low-Level Design: Detailed specification of modules within the architecture.
Programming: Coding of the modules.

## Defect Prevention
Techniques include:
Instrumentation code.
Handling return values, counter data fields, buffer overflow/underflow.
Common source for error messages and help texts.
Validating input data.
Using assertions to detect impossible conditions.
Reverse-computing inputs from results.
Loop counters in each loop.

## Mutation Testing
Mutant: Modified program with a single change.
Mutation Test: Testing process involving mutants.
Definitions: Mutant, Killed Mutant, Dead Mutant, Equivalent Mutant, Killable/Stubborn Mutant, Mutant-adequate test suite.

## Data Flow Anomalies
Defined and defined again (type 1).
Undefined but referenced (type 2).
Defined but not referenced (type 3).

## Data Flow Testing
Visualizes the "flow" of data values from one statement to another.
Motivations:
Perform tests on data values produced in one statement and used later.

## Domain Error
Input domain: Set of all input data to the program.
Program path: Sequence of instructions from entry to exit.
Feasible path: Exists input data causing the path to execute.
Infeasible path: No input data causes the path to execute.
Errors:
Computation Error: Correct path, wrong output.
Domain Error: Wrong path executed for specific input data.
A program with domain errors misclassifies inputs, leading to incorrect path execution.
