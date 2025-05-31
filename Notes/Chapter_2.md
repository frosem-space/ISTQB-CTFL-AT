<p align="center"> <a href="https://www.istqb.org/certifications/certified-tester-foundation-level-agile-tester-ctfl-at/" title="Certified Tester Foundation Level Agile Tester (CTFL-AT)"> <img src="https://www.istqb.org/wp-content/uploads/2024/10/istqb-agile-tester-logo.jpg.avif" width="200" alt="ISTQB CTFL-AT Logo"/></img> </a> </p>


# Chapter 2: Fundamental Agile Testing Principles, Practices, and Processes


## 2.1 The Differences Between Testing in Traditional and Agile Approaches

Agile and traditional lifecycles (e.g., sequential such as the
V-model or iterative such as RUP) differ significantly in how testing activities are integrated. Testers in Agile must understand these differences to work effectively, especially since practices vary between organizations.

Adaptability is essential: even when practices deviate from Agile ideals, those changes may be context-driven and intelligent.

### 2.1.1 Testing and Development Activities

Agile development is structured around short iterations that each produce working software. Planning is done at both release and iteration levels.

Testing occurs throughout each iteration — not at the end. Development, integration, and testing happen in parallel.

- Developers perform unit testing during feature implementation.
- Testers verify the completed features.
- Business stakeholders also test to provide immediate feedback.

Some teams use “hardening” iterations to resolve defects or technical debt, although best practice is to finish each feature fully within its own iteration. A “fix bugs first” approach can be used, where defects from one iteration are handled early in the next. This can complicate effort estimation.

Release activities may follow the full iteration cycle, or happen at the end of each iteration.

When using risk-based testing, testers lead high-level risk analysis during release planning and more detailed assessments during iteration planning. This affects development order, test depth, and effort estimation.

### Pairing and Collaboration

Agile often uses pairing:
- Two testers working together on a feature.
- A tester and a developer collaborating during development and testing.

While distributed teams can make pairing harder, tools can support this collaboration. Testers also serve as coaches, sharing testing knowledge and promoting team-wide quality ownership.

### Test Automation and Experience-Based Testing

Agile relies heavily on automated testing at all levels. Testers may:
- Create and maintain automated integration and system tests.
- Use exploratory and defect-based techniques for manual testing.

While developers will focus on creating unit tests, testers should focus on creating automated integration, system, and system integration tests. This leads to a tendency for Agile teams to favor testers with a strong technical and test automation background.

Since Agile embraces change, lightweight documentation is preferred. Automated testing helps manage regression risks from frequent changes. However, the rate of change must stay within the team’s capacity to manage risks effectively.

### 2.1.2 Project Work Products

Agile testers interact with three main types of work products:

1. **Business-oriented**: What is needed and how to use it (e.g., user stories, acceptance criteria, user documentation).
2. **Development-related**: How the system is built (e.g., code, unit tests, technical diagrams).
3. **Testing-related**: How the system is tested and the outcomes (e.g., test plans, test results, defect reports).

Agile emphasizes minimizing unnecessary documentation while ensuring enough is available for development, testing, and maintenance.

### Business Work Products

User stories describe small, testable features and are usually created during planning. Larger stories are called **epics** and are broken down over multiple sprints. Stories can include both UI-level (application) and API-level (middleware) requirements. Acceptance criteria are linked to each story or epic.

### Developer Work Products

Developers produce code and automated unit tests. In test-driven development (TDD), they write tests before the code. In reality the tests are more a form
of executable low-level design specifications rather than tests.

### Tester Work Products

Testers produce:
- Automated tests
- Test plans and risk catalogs
- Manual test cases
- Defect reports and test logs
- Lightweight metrics based on test execution

In regulated or complex projects, additional formal documentation may be required. This includes traceability matrices and detailed specifications derived from user stories to satisfy auditors, regulations and other requirements.

## 2.1.3 Test Levels

In Agile, Test levels are test activities that are logically related, test activities are structured around the progression of a user story during an iteration. These levels often overlap due to the iterative nature of development.

### A typical flow during an iteration includes:

- **Unit testing**: Done by developers during feature implementation.
- **Feature verification testing**: Often automated and executed by developers or testers, based on the acceptance criteria.
- **Feature validation testing**: Usually manual and involves developers, testers, and business stakeholders to assess whether the feature is fit for use.

In parallel, regression testing is performed throughout the iteration. This involves re-running unit and verification tests from current and previous iterations, usually through continuous integration.

Some teams also apply **system-level testing** once enough features are implemented. This includes functional and non-functional testing (e.g., performance, usability, reliability).

Acceptance testing types used in Agile include:

- Internal alpha tests
- External beta tests
- User acceptance testing
- Operational, regulatory, and contract acceptance testing

These may occur at the end of an iteration or after a group of iterations.

## 2.1.4 Testing and Configuration Management

Agile teams make heavy use of automated tools for development and testing. Developers use static analysis, unit test tools, and coverage tools. All code and unit tests are continuously integrated into a shared repository, with automated builds and tests triggered on check-in.

Functional tests at integration and system level may also be automated, using open-source or commercial tools. These are typically run less frequently than unit tests, due to longer execution times.

The goal is to maintain a working, installable build at all times. If any automated test fails, the issue should be fixed before the next check-in. This prevents inefficient cycles of broken builds and failed installs.

Automation helps reduce the risk associated with frequent changes. However, relying solely on unit tests is not enough, since they have limited defect detection. Integration and system-level tests are also needed to manage regression risks effectively.

## 2.1.5 Organizational Options for Independent Testing

Independent testing is valuable but must be adapted to Agile.

### Common approaches include:

1. **Embedded testers** within Agile teams: Testers work directly with developers and stakeholders. This speeds up feedback but may reduce independence and objectivity.

2. **On-demand independent testers**: A separate test team performs testing near the end of the sprint. This can preserve independence, but time constraints and weak product knowledge often limit effectiveness.

3. **Long-term assignment of independent testers**: Testers from a separate test group join Agile teams from the start and stay long term. This balances independence with deep team integration and understanding.

Additionally, some independent testers may remain outside of Agile teams and focus on:

- Developing and maintaining test tools
- Performing non-functional tests
- Creating test environments and data
- Carrying out test levels that might not fit well within a sprint (e.g., system integration testing).


## 2.2 Status of Testing in Agile Projects

Agile projects evolve quickly, which means test progress and product quality are constantly changing. Testers must keep the team informed so they can make decisions on time. Manual and automated tests must be frequently updated to manage regression risks effectively.

### 2.2.1 Communicating Test Status, Progress, and Product Quality

In Agile, the goal is to deliver working software at the end of each iteration. To support this, test progress is tracked and shared using various tools and methods, such as:

- Test automation results
- Task board updates
- Burndown charts
- Dashboards or status emails
- Verbal updates during stand-up meetings

Burndown charts track remaining work across the release or iteration. 

The story cards, development tasks, test tasks, and other tasks created during **iteration planning**.

Task boards reflect current status using columns like *to do*, *in progress*, *verify*, and *done*. Color-coded task cards show development and test tasks separately.

Testing tasks are directly tied to the acceptance criteria of user stories. As test cases (automated, manual, exploratory) are completed, they move through the task board. The team reviews task board status daily in stand-up meetings.

Each team member answers:
- What did you complete since the last meeting?
- What will you complete before the next?
- What’s blocking your progress?

Any issues that may block test progress are communicated during the daily stand-up meetings, so the whole team is aware of the issues and can resolve them accordingly.

To evaluate and improve quality, Agile teams may collect metrics such as:
- Test pass/fail rates
- Confirmation and Regression test result
- Defect discovery and resolution rates
- Requirements and risk coverage
- Code coverage and churn

These metrics help inform decisions but should never be used to reward or punish any team members.

### 2.2.2 Managing Regression Risk with Evolving Manual and Automated Test Cases

As the product grows with each iteration, the risk of regression increases. Code churn and changes to previous features introduce this risk. To manage it, teams must:

- Maintain and update manual and automated test cases
- Store all test artifacts (cases, data, scripts) in version-controlled tools
- Review and refactor test cases regularly
- Identify outdated or obsolete tests
- Add new tests to cover changes

Testers must select which cases to include in the regression suite and retire irrelevant ones. They also need to assess whether tests can or should be automated.

Automated regression tests reduce effort and allow testers to focus on new features. Test cases must be traceable and easily modifiable to reflect product changes.

During release planning, the team should define:
- How test cases are written and stored
- Standards for test design and maintenance

Well-managed test design is critical given the fast pace and frequent change.

### Test Automation and Build Integration

Automated unit tests should pass before code is checked in. This prevents breaking the build and slows down the team.

Automated acceptance tests run against complete system builds—usually daily. 

They offer feedback on regression but not overall product quality. A subset of these, called **build verification tests**, run immediately after deployment to catch major issues early.

If an automated regression test fails:
- It may reflect a real defect → fix it
- It may be outdated → update or replace it
- It may overlap with another test → retire it

Additional test tasks that can be automated include:
- Generating and loading test data
- Deploying builds
- Resetting test environments to a baseline
- Comparing data outputs

Automating these tasks reduces repetitive work and allows the team to focus on testing current features.

## 2.3 Role and Skills of a Tester in an Agile Team

Testers in Agile teams work closely with developers and business stakeholders. This requires both technical and interpersonal skills, as well as active participation across planning, development, and delivery.

### 2.3.1 Agile Tester Skills

In addition to the general skills expected of all testers, Agile testers are expected to be competent in:

- Test automation
- Test-driven development (TDD)
- Acceptance test-driven development (ATDD)
- White-box, black-box, and experience-based testing

Since Agile emphasizes collaboration, communication, and interaction between the team members as well as stakeholders outside the team, interpersonal skills are essential.

Agile testers should:
- Be positive, solution-oriented, and collaborative
- Think critically and focus on quality
- Actively acquire information from stakeholders
- Accurately evaluate and report test results, test progress and product quality
- Help define testable user stories and acceptance criteria
- Work in pairs with developers and other team members
- Adapt quickly to changes in requirements or features
- Organize and plan their own testing tasks

Testers must continue developing both technical and interpersonal skills over time.

### 2.3.2 The Role of a Tester in an Agile Team

Testers in Agile teams provide feedback not just on the test status, test progress, and the quality of the product, but also on test and process quality. Their role includes:

- Maintaining and updating the team’s test strategy
- Measuring and reporting test coverage
- Managing and using testing tools effectively
- Setting up and maintaining test environments and test data
- Reporting defects and collaborating to resolve them
- Coaching other team members on testing concepts
- Ensuring that appropriate testing tasks are included in release and iteration planning
- Working with developers and business representatives to clarify requirements, especially in terms of testability, consistency, and completeness
- Contributing to retrospectives by suggesting improvements

All team members share responsibility for product quality and may be involved in test-related tasks.

### Organizational Risks

Agile teams may face risks related to the tester’s role, such as:

- Loss of independent mindset due to close collaboration with developers
- Tolerance or silent about inefficient, ineffective, or low-quality practices within the team
- Inability to keep up with fast-paced changes in short iterations

To manage these risks, organizations may adopt independent testing approaches discussed in Section 2.1.5.

