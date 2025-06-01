<p align="center"> <a href="https://www.istqb.org/certifications/certified-tester-foundation-level-agile-tester-ctfl-at/" title="Certified Tester Foundation Level Agile Tester (CTFL-AT)"> <img src="https://www.istqb.org/wp-content/uploads/2024/10/istqb-agile-tester-logo.jpg.avif" width="200" alt="ISTQB CTFL-AT Logo"/></img> </a> </p>


# 3. Agile Testing Methods, Techniques, and Tools

## 3.1 Agile Testing Methods

Agile encourages early testing and quality activities across the lifecycle. Practices such as defining tests before coding, preventing defects early, and running the right tests at the right level and time are central. Testers help introduce and apply these practices from the beginning of the project.

### 3.1.1 Test-Driven Development, Acceptance Test-Driven Development, and Behavior-Driven Development

Agile teams apply several development-driven testing techniques that define tests before writing code. These practices support early defect detection and reinforce collaboration.

#### Test-Driven Development (TDD)

TDD focuses on developing code through short cycles of writing tests and code. The process:

1. Write a test that defines expected behavior.
2. Run the test and confirm it fails.
3. Write the code and run the test in a tight loop until the test passes.
4. Refactor the code and rerun the test.
5. Repeat the process with additional tests.

TDD produces automated unit-level tests, sometimes used at integration or system levels. It supports continuous integration and helps clarify expected results during development.

#### Acceptance Test-Driven Development (ATDD)

ATDD defines acceptance criteria and tests during user story creation. It is a collaborative process involving developers, testers, and business stakeholders.

- Acceptance tests are created before development starts.
- Tests can be reused for regression testing.
- Tools support execution of acceptance tests within the continuous integration pipeline.
- Allows quick resolution of defects and validation of feature behavior
- Tests often interact with system or service layers to verify behavior.

ATDD helps validate feature behavior and ensures acceptance criteria are met.

#### Behavior-Driven Development (BDD)

BDD focuses on writing tests based on expected software behavior using plain, structured language. Tests are written in a format that’s understandable to the whole team.

Typical BDD format:
- **Given** a specific context
- **When** an action is taken
- **Then** an outcome is expected

BDD supports collaboration, especially when defining unit tests that reflect business needs. Frameworks can generate test code from these definitions.

### 3.1.2 The Test Pyramid

The test pyramid describes how tests should be distributed across test levels:

- **Bottom**: Unit tests (high volume)
- **Middle**: Integration tests (moderate volume)
- **Top**: System and acceptance tests (low volume)

The pyramid emphasizes having more tests at the lower levels to catch defects early. Lower-level tests (unit, integration) are typically automated using API-based tools. Upper-level tests (system, acceptance) are usually automated with GUI-based tools.

This model aligns with the principle of early quality assurance: detecting and fixing issues early in the lifecycle is more efficient and cost-effective.

### 3.1.3 Testing Quadrants, Test Levels, and Testing Types

The testing quadrants help align test levels and test types in Agile. They provide a clear way to organize testing activities and make them understandable to all stakeholders.

Tests may be business-facing or technology-facing. Some support development; others verify product quality. Tests can be manual, automated, or a combination.

- **Q1**: Unit level, technology-facing, supports developers. Includes unit tests, automated and integrated into continuous integration.
- **Q2**: System level, business-facing, confirms product behavior. Includes functional tests, examples, story tests, UX prototypes. Can be manual or automated.
- **Q3**: System or acceptance level, business-facing, critiques the product. Includes exploratory testing, scenarios, usability testing, UAT, alpha/beta testing. Typically manual.
- **Q4**: System or operational acceptance level, technology-facing, critiques the product. Includes performance, load, stress, security, compatibility, and recovery tests. Often automated.

Tests from multiple quadrants may be applied in a single iteration. The model focuses on dynamic testing, not static analysis.

### 3.1.4 The Role of a Tester

Agile testers participate throughout the lifecycle, especially in Scrum. Their role includes collaborative planning, executing, and reviewing of tests and supporting team goals.

#### Teamwork in Scrum

Agile relies on collaboration between developers, testers, and business stakeholders. Effective Scrum teams follow practices such as:

- **Cross-functional**: Each team member brings a different set of skills to the team. The team works together on test strategy, planning, specification, execution, evaluation, and results reporting.
- **Cross-functional**: All skills are represented; testing responsibilities are shared.
- **Self-organizing**: Teams structure their work and include testers as needed.
- **Co-located**: Testers work closely with the team and product owner.
- **Collaborative**: Open communication with team, stakeholders, and Scrum Master.
- **Empowered**: Teams make design and test decisions together.
- **Committed**: Testers actively evaluate product behavior and customer needs.
- **Transparent**: Progress is tracked visibly on the task board.
- **Credible**: Stakeholders trust test results when the strategy is clear and consistent.
- **Open to feedback**: Teams improve through retrospectives.
- **Resilient**: Testers adapt to change, as required in Agile.

#### Sprint Zero

Sprint Zero is the initial setup sprint where preparation activities take place. The tester collaborates on:

- Identify the scope of the project (i.e., product backlog).
- Create initial system architecture and high-level prototypes.
- Selecting and installing tools (test management, defect management, test automation, CI).
- Creating the initial test strategy for all test levels, test scope, technical risks, test types, and coverage goals.
- Performing a initial quality risk analysis.
- Defining test metrics to measure the test process and quality.
- Specify the “definition of done”.
- Creating the task board.
- Defining conditions for ending testing.

Sprint Zero sets the foundation for all future testing activities.

#### Integration

To support continuous delivery of value, testing must be integrated into development. The integration strategy should identify dependencies and enable continuous testing across features.

#### Test Planning

Test planning begins during release planning and continues through each sprint. Plans are updated frequently and broken into manageable tasks (typically 1–2 days). All test-related issues must be tracked and addressed during the sprint.

#### Agile Testing Practices

Useful practices for Agile testers include:

- **Pairing**: Two team members collaborate on testing tasks (e.g., tester-developer, tester-product owner).
- **Incremental test design**: Tests cases and charters are gradually built from simple to complex based on user stories.
- **Mind mapping**: Visual tool to plan test sessions, data, and strategies.

### 3.2 Assessing Quality Risks and Estimating Test Effort

Testing helps reduce product quality risks to an acceptable level. Agile testers use traditional risk analysis and estimation techniques but must adapt them to fast-paced, short-iteration environments.

### 3.2.1 Assessing Quality Risks in Agile Projects

Agile testers support prioritization and test effort allocation by identifying and assessing quality risks.

Risk Level = likelihood of a problem × impact of that problem.  
- **Quality risks** affect the product.
- **Project risks** affect delivery success.

Risk analysis happens at two levels:
- **Release planning**: Business representatives and the team identify high-level risks.
- **Iteration planning**: The full team assesses quality risks tied to each backlog item.

Examples of quality risks:
- Incorrect calculations in reports (functional risk, accuracy)
- Slow system response (non-functional risk, performance)
- Difficulty in understanding screens and fields (non-functional risk, usability)

Tasks linked to high-risk items should be prioritized and receive more testing effort.

A typical risk analysis flow in iteration planning includes:
1. Gather the team together.
2. Review backlog items.
3. Identify quality risks per item.
4. Assess and categorize risks by imapct and likelihood of defects.
5. Allocate test effort based on risk level.
6. Choose test techniques that best mitigate each risk.

Testers design, implement, and run tests targeting these risks. While risk analysis is ongoing, new risks can appear, and existing ones may change in priority or severity. Test strategies must adapt accordingly.

Risk mitigation may also happen before test execution, for example by reviewing and improving user stories early.

### 3.2.2 Estimating Testing Effort Based on Content and Risk

Effort estimation includes testing and is part of release planning. Agile teams often use **planning poker** to estimate effort collaboratively.

- Each team member selects a card (typically using the Fibonacci sequence) to represent their estimate of effort.
- Larger numbers indicate higher uncertainty or larger tasks.
- Estimates may be in story points, effort days, or other units.

Process:

1. Product owner presents a user story.
2. Estimators discuss the story and ask questions.
3. All estimators reveal their estimates at once.
4. If estimates match, it becomes the agreed estimate.
5. If not, estimators discuss, then repeat until consensus is reached or a rule is applied (e.g., median value).

Testing effort should consider:
- Complexity of the feature
- Scope and type of testing required
- Level of associated risk

Including risk levels in planning helps provide more accurate effort estimates and better understanding of work required for each item.

### 3.3 Techniques in Agile Projects

Many testing techniques from traditional lifecycles also apply to Agile, but Agile projects introduce specific practices and variations in terminology, documentation, and execution.

### 3.3.1 Acceptance Criteria, Adequate Coverage, and Other Information for Testing

User stories are the primary test basis in Agile. They are typically brief and follow a defined structure. Non-functional requirements (e.g., usability, performance) can be included as standalone stories or tied to functional stories.

Other useful test bases include:

- Experience from previous projects
- Existing system functionality
- Code, architecture, and design
- User profiles and environments
- Known defects and defect categories
- Standards and regulations
- Quality risk analysis

Acceptance criteria help verify that user stories are implemented correctly. Criteria should consider:

- Functional behavior
- Quality characteristics (performance, reliability, etc.)
- Scenarios and use cases
- Business rules
- External interfaces
- Constraints (e.g., hardware limits)
- Data definitions (e.g., format, value ranges)

Testers also need information about:
- System usage
- Interface access
- Tool support
- Whether they have sufficient knowledge.

Information gaps discovered during the iteration should be resolved through collaboration.

#### Test Levels

The **definition of done** determines when work is considered complete, and applies at multiple levels:

#### Unit Testing

- 100% decision coverage where feasible
- Static code analysis complete
- No unresolved major defects or technical debt
- Code, tests, and results reviewed
- Tests automated and performance within limits

#### Integration Testing

- All functional requirements covered, including negative tests
- All interfaces between units tested
- All quality risks covered as planned
- No unresolved major defects
- Defects reported
- Regression tests automated and stored centrally

#### System Testing

- End-to-end tests for user stories and features
- All user personas covered
- Critical quality attributes tested (performance, reliability)
- Testing in production-like environments
- Regression tests automated and stored
- No unresolved major defects

#### User Story Level

- Stories are complete, testable, and understood with detailed acceptance criteria
- Acceptance tests specified and reviewed
- Tasks identified and estimated

#### Feature Level

- All related user stories defined and approved by the customer
- Design and code complete with no technical debt
- Unit, integration, and system tests executed with required coverage
- No major defects
- Documentation completed (e.g., release notes, user manuals)

#### Iteration Level

- All features tested and meet feature-level done criteria
- Non-critical unresolved defects added to backlog
- Integrated and tested feature set
- Documentation written and reviewed

The software may now be considered potentially releasable.

#### Release Level

Criteria to declare a release done may include:

- **Coverage**: All relevant test items are covered; adequacy based on size, complexity, and risk.
- **Quality**: Defect rates, densities, and remaining risks are within acceptable limits.
- **Time**: The delivery date has been reached and business considerations evaluated.
- **Cost**: Return on investment is justified based on development and maintenance costs compared to expected revenue.

Maintaining quality post-release is important to limit maintenance cost due to escaped defects.

### 3.3.2 Applying Acceptance Test-Driven Development

Acceptance test-driven development (ATDD) is a test-first approach. Tests are created before coding begins. These tests are written collaboratively by developers, testers, and business representatives.

The process starts with a **specification workshop**, where the team clarifies and improves the user story. Afterward, the team creates examples that act as acceptance tests. These can be manual or automated.

- Positive path tests are created first, followed by negative cases and non-functional attributes.
- Tests are written in natural language to ensure understanding by all stakeholders.
- Each example must map directly to a characteristic in the user story, without duplication or introducing new scope.

These tests help verify implementation and guide development by setting clear expectations.

### 3.3.3 Functional and Non-Functional Black Box Test Design

Testers often create black box tests during development, using the same user stories and acceptance criteria as developers.

Standard black box techniques include:

- Equivalence partitioning
- Boundary value analysis
- Decision tables
- State transition testing

These techniques apply to both **functional** and **non-functional** requirements. Non-functional criteria (e.g., performance, reliability) are often written as user stories.

Example:
- A performance user story may require response time under 2 seconds.
- A reliability story may limit failure rates.

These methods help design effective and focused test cases, whether for functionality or quality attributes.

### 3.3.4 Exploratory Testing and Agile Testing

Exploratory testing is valuable in Agile due to short timelines and limited story details. It works best when combined with other strategies such as:

- Risk-based testing
- Requirements-based testing
- Model-based testing
- Regression-averse testing

**Exploratory testing** blends test design and execution, guided by a **test charter**. A test charter outlines:

- Actor: who is using the system
- Purpose: test objectives
- Setup: environment or preconditions
- Priority: importance of the charter
- Reference: supporting docs, risks, or requirements
- Data: inputs needed for testing
- Activities: what the tester will do (e.g., actions to try)
- Oracle notes: how to evaluate expected results
- Variations: alternate actions or outcomes

**Session-based test management** is often used:
- Each session is 60–120 minutes
- Sessions can focus on:
    - Survey session (to learn how it works)
    - Analysis session (evaluation of the functionality or characteristics)
    - Deep coverage (corner cases, scenarios, interactions)

Exploratory testers rely on creativity, system understanding, and relevant domain knowledge. Good exploratory questions include:
- What is most important to find out about the system?
- What might fail here?
- What should happen in this situation?
- Are user expectations being met?

**Heuristics** guide exploration. Examples:
- Boundaries
- CRUD (Create, Read, Update, Delete)
- Configuration changes
- Interruptions (e.g., log off, restart)

Testers must document what they do. Suggested documentation includes:

- **Test coverage**: what was tested and what remains.
- **Evaluation notes**: stability, observations, next steps.
- **Risk and strategy tracking**: which risks have been covered and which ones remain.
- **Issues and anomalies**: any unexpected behavior, any questions regarding the efficiency of the approach, any concerns about the ideas/test attempts.
- **Actual behavior**: saved via screenshots, logs, or recordings

Documentation should be summarized in a tool (e.g., test/task management board) so stakeholders can easily understand testing progress and outcomes.

### 3.4 Tools in Agile Projects

Agile teams use tools that are sometimes used differently or with greater relevance. For example, some teams prefer all-in-one tools that combine test management, requirements tracking, task boards, and burndown charts. Configuration management tools are essential for handling the many automated tests and related assets in Agile environments.

In addition to traditional tools, Agile testers may use specific tools that support collaboration and information sharing across the team.

### 3.4.1 Task Management and Tracking Tools

Agile teams may use physical boards (whiteboards, corkboards) or digital tools (e.g., task management or application lifecycle management systems). These tools help:

- Record user stories and their related development and test tasks
- Capture estimates and calculate overall effort for each story
- Link development and test tasks to the same story for a complete view of work
- Track task progress and provide real-time status updates at the story, sprint, and release level
- Display visual metrics, dashboards, and charts for easy status review by all team members
- Integrate with version control tools to track code check-ins, builds, and automatically update task status

These tools provide visibility into team progress and support coordination, especially in distributed teams.

### 3.4.2 Communication and Information Sharing Tools

Agile teams use a variety of tools to facilitate communication and knowledge sharing beyond email and direct conversations:

#### Wikis

Used to share project-related knowledge, including:
- Product features, diagrams, prototypes, and team discussions
- Useful development and testing tools or techniques
- Automatically updated charts and dashboards linked to task or build tools
- Asynchronous team conversations documented and shared

#### Instant Messaging and Video Tools

These tools support:
- Real-time communication for distributed teams
- Remote participation in daily standups and team meetings
- Reduced communication costs using voice-over-IP

#### Desktop Sharing and Capture Tools

These allow:
- Remote code reviews, demos, and pairing
- Recording and sharing sprint-end product demonstrations via wiki or internal portals

These tools support but do not replace face-to-face communication. They help maintain strong collaboration in Agile teams, particularly when working across locations.

### 3.4.3 Software Build and Distribution Tools

Agile teams rely on daily builds and frequent deployments, which require continuous integration and build distribution tools. These tools help:

- Build the application frequently
- Detect integration issues early
- Automate deployment into test environments

### 3.4.4 Configuration Management Tools

Configuration management tools are used to store not only source code but also automated tests, manual tests, and other test artifacts. This ensures:

- Traceability between code and the specific test versions used
- Support for rapid change while preserving historical data

Agile teams may use either:

- **Centralized version control systems**
- **Distributed version control systems**

The choice depends on team size, structure, location, and integration needs with other tools.

### 3.4.5 Test Design, Implementation, and Execution Tools

Various tools support different stages of the Agile testing process:
- **Test design tools**: Mind maps and visual models help quickly define tests for new features.
- **Test case management tools**: Often integrated into lifecycle or task management tools used by the whole team.
- **Test data preparation and generation tools**: Help generate and maintain complex data. These tools may use production data (after anonymization) or create large data sets for load testing.
- **Test data load tools**: Automatically load test data into applications, reducing manual effort and errors.
- **Automated test execution tools**: Support Agile practices like BDD, TDD, and ATDD. These tools often let testers and business users define tests in natural language or structured formats.
- **Exploratory testing tools**: Capture user actions during exploratory sessions, aiding in defect reproduction and regression suite creation.

These tools improve efficiency and adaptability in fast-changing Agile environments.

### 3.4.6 Cloud Computing and Virtualization Tools

Virtualization and cloud technologies allow Agile teams to:

- Create and manage virtual machines for development and testing
- Provision or restore environments quickly using snapshots
- Reduce delays caused by limited hardware resources

Some test management tools integrate with virtualization platforms to capture a snapshot when a defect is found. This snapshot can then be shared with developers for analysis, improving debugging and resolution speed.

