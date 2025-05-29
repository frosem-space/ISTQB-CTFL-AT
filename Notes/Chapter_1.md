<p align="center"> <a href="https://www.istqb.org/certifications/certified-tester-foundation-level-agile-tester-ctfl-at/" title="Certified Tester Foundation Level Agile Tester (CTFL-AT)"> <img src="https://www.istqb.org/wp-content/uploads/2024/10/istqb-agile-tester-logo.jpg.avif" width="200" alt="ISTQB CTFL-AT Logo"/></img> </a> </p>


# Chapter 1: Agile Software Development


# 1.1 The Fundamentals of Agile Software Development

Agile testers work differently from those in traditional projects. They must understand Agile values and principles, and collaborate closely with developers and business representatives. Early and frequent communication helps eliminate defects early and deliver high-quality products.

## 1.1.1 Agile Software Development and the Agile Manifesto

In 2001, the Agile Manifesto was created, establishing four core values:

- Individuals and interactions *over* processes and tools  
- Working software *over* comprehensive documentation  
- Customer collaboration *over* contract negotiation  
- Responding to change *over* following a plan  

Although the items on the right have value, Agile values those on the left more.

### Key Concepts Behind Each Value

1. **Individuals and Interactions**: Emphasizes communication and collaboration over reliance on tools.  
2. **Working Software**: Prioritizes delivering usable functionality early, allowing quick feedback and faster time-to-market.  
3. **Customer Collaboration**: Close, continuous interaction with customers improves requirement clarity and project outcomes.  
4. **Responding to Change**: Agile embraces change rather than resisting it, allowing adaptation to external factors like business shifts or technological advances.

### Agile Principles

The Agile Manifesto is supported by twelve guiding principles:

1. Deliver valuable software early and continuously.
2. Welcome changing requirements, even late in development.
3. Deliver working software frequently (weeks to months).
4. Business and developers must work together daily.
5. Build projects around motivated individuals with proper support.
6. Face-to-face communication is the most effective method.
7. Working software is the primary measure of progress.
8. Promote sustainable development at a constant pace.
9. Maintain technical excellence and good design.
10. Simplicity is essential—maximize work not done.
11. Self-organizing teams produce best architectures, requirements, and designs.
12. Teams regularly reflect and improve their effectiveness.

Agile methodologies apply these values and principles through specific practices.

## 1.1.2 Whole-Team Approach

The whole-team approach involves everyone  with the knowledge and skills necessary for project success, including testers, developers, and business stakeholders. Teams are ideally small (3–9 people) and co-located to improve communication.

Daily stand-ups help identify progress and impediments.

### Benefits of the Whole-Team Approach

- Enhances collaboration and communication.
- Leverages diverse skill sets across the team to benefit the project.
- Assigns responsibility for quality to the entire team.

## Testers actively participate in all stages, including:

- Supporting business stakeholders in defining acceptance tests.
- Collaborating with developers on testing strategy.
- Contributing to decisions on test automation.

All team members, including testers, are involved in feature discussions, estimates, and decisions. This practice is known as the **"power of three"**, involving testers, developers, and business representatives working closely together, the quality level is a shared responsibility.

## 1.1.3 Early and Frequent Feedback

Agile projects use short iterations to enable early and continuous feedback on product quality throughout the development lifecycle. One way to provide rapid feedback is by continuous integration.

Unlike sequential development where customers only see the final product, Agile teams collect regular feedback throughout development. This enables early adjustments, helps prioritize high-value features, and improves transparency by showing sprint capacity and velocity improvements. 

For example, how much work can we do in a sprint or iteration? What could help us go faster? What is preventing us from doing so?

### Benefits of Early and Frequent Feedback

1. Helps avoid misunderstandings in requirements by identifying issues earlier.
2. Allows early clarification and delivery of requested features to the customer.
3. Enables early detection and resolution of quality issues through continuous integration.
4. Provides transparency into team performance and delivery capacity.
5. Supports better planning and adjustments to improve team velocity.
6. Maintains consistent momentum throughout the project.

Frequent feedback ensures that high-value and high-risk features are prioritized and delivered first, improving customer satisfaction and reducing rework.

# 1.2 Aspects of Agile Approaches

Agile organizations use a variety of practices such as collaborative user story creation, retrospectives, continuous integration, and both iteration and release planning.

## 1.2.1 Agile Software Development Approaches

Agile values and principles are implemented through multiple frameworks, this syllabus focuses on three: Extreme Programming (XP), Scrum, and Kanban.

### Extreme Programming (XP)
XP emphasizes five core values: communication, simplicity, feedback, courage, and respect.

It also promotes principles like humanity, economics, mutual benefit, self-similarity, improvement, diversity, reflection, flow, opportunity, redundancy, failure, quality, baby steps,
and accepted responsibility.

XP outlines thirteen primary development practices, including: sit together, whole team, informative workspace, energized work, pair programming, stories, weekly cycle, quarterly cycle, slack, ten-minute build, continuous integration, test first programming, and incremental design.

XP has influenced many other Agile frameworks, including Scrum.

### Scrum
Scrum is an Agile framework focused on project and team management, based on:
- **Sprints**: Fixed-length iterations (2–4 weeks).
- **Product Increment**: Deliverable product at the end of each sprint.
- **Product Backlog**: Prioritized list of features maintained by the Product Owner.
- **Sprint Backlog**: Selected items for the current sprint, based on pull principle.
- **Definition of Done**: Shared understanding of when work is considered complete.
- **Timeboxing**: Fixed time limits to tasks for sprints and meetings.
- **Transparency**: Daily scrums and visible product status to the team.

Scrum defines three main roles:
- **Scrum Master**: Facilitator and guardian of Scrum practices.
- **Product Owner**: Voice of the customer, manages and prioritizes the product backlog.
- **Development Team**: Self-organizing, cross-functional team that builds and tests the product.

Scrum does not prescribe specific testing techniques or software engineering practices.

### Kanban
Kanban is a visual workflow management method that emphasizes flow and continuous delivery without mandatory sprints.

It uses three primary mechanisms:
- **Kanban Board**: A visual workflow board with columns showing stages like development and testing, where tasks move across as tickets.
- **Work-in-Progress Limits**: Each stage has maximum task limits. New work starts only when capacity allows.
- **Lead Time**: Measures and optimizes the time to complete tasks through the workflow.

Kanban and Scrum both use visual task tracking for transparency, with tasks moving from backlog to board when capacity allows. Kanban differs by making iterations optional and allowing single-item releases, while Scrum requires synchronized sprints.

## 1.2.2 Collaborative User Story Creation

In Agile, requirements are captured as user stories. These are created collaboratively by developers, testers, and business representatives, this shared vision is accomplished through frequent informal reviews while the requirements are being written.

In sequential development, this shared vision of a feature is accomplished through formal reviews after requirements are written.

### Key Concepts
- User stories cover both functional and non-functional aspects.
- The acceptance criteria should be defined in collaboration between business representatives, developers, and testers. 
- The team considers a task finished when a set of acceptance criteria have been satisfied.
- Testers contribute by identifying gaps in the user story (missing details or non-functional requirements), by asking business representatives open-ended questions and confirming testability of the acceptance criteria.

### Techniques
- **Brainstorming and mind mapping** help in collaborative authorship story creation.
- **INVEST** criteria define quality user stories:
  - Independent
  - Negotiable
  - Valuable
  - Estimable
  - Small
  - Testable

### 3C Model
- **Card**: Describes the story identifying the requirements, criticality, expected development/test duration and the acceptance criteria.
- **Conversation**: Facilitates shared understanding on how the software will be used, the team members brings valuable input to the exchange of thoughts, opinions and experiences.
- **Confirmation**: Validates completion through acceptance tests. Both positive and negative tests should be used to cover the criteria. During confirmation, various participants play the role of a tester.

Documentation should be minimal but concise, sufficient, and necessary.

## 1.2.3 Retrospectives

In Agile, a retrospective is a meeting held at the end of each iteration to discuss what worked, what didn’t, and what to improve.

### Purpose and Scope
- Topics include team dynamics, tools, processes, and relationships.
- Aim to support continual improvement in a trusted environment.

### Tester Involvement
- It can result in test-related improvement decisions focused on test effectiveness, test productivity, test case quality, and team satisfaction.
- Testers are part of the team and bring their unique perspective.
- All team members, testers and non-testers, can provide input on both testing and non-testing activities.

## 1.2.4 Continuous Integration

In Agile, continuous integration is used to ensure that software is always in a working, testable state. All changes are merged and integrated frequently, at least once per day.

### Automated activities include:
- **Static code analysis**: Running analysis tools.
- **Compile**: Creating executable files.
- **Unit test**: Running tests and measuring coverage.
- **Deploy**: Installing in test environment.
- **Integration test**: Running integration tests.
- **Report**: Publishing status to dashboard/email.

This automation allows early detection of integration errors, provides fast feedback on code quality, and supports test execution throughout the sprint.

Agile testers can focus manual testing on new features and defect fixes while relying on automated regression tests for previously delivered functionality.

Additional tools can enhance quality control by executing performance tests, generating documentation, and automating deployments across environments.

### Benefits of continuous integration include:

1. Faster detection and root cause analysis of integration issues.
2. Regular feedback to the team on software stability.
3. Keeps the version between development and testing within a day.
4. Reducing risk from refactoring through rapid re-testing.
5. Daily confirmation that the software remains stable.
6. Making progress visible, which helps maintain motivation.
7. Eliminating the risk of last-minute "big bang" integration.
8. Ensuring testable, deployable software is always available.
9. Reducing repetitive manual testing.
10. Providing faster feedback on quality decisions.

### Risks and challenges include:

1. Need for ongoing setup and maintenance of integration tools.
2. Complexity in defining and maintaining the integration process.
3. Effort required to establish automated tests and maintain coverage.
4. Overreliance on unit tests, with insufficient system and acceptance testing

Effective use of continuous integration requires tools for version control, build automation, deployment, and test automation.

## 1.2.5 Release and Iteration Planning

Agile planning involves two levels: **release planning** and **iteration planning**.

### Release Planning

Release planning focuses on defining the product backlog and planning across multiple iterations. It may span months ahead and helps form a high-level test approach.

### Tester contributions in release planning include:

- Defining testable user stories with clear acceptance criteria.
- Participating in project and quality risk analysis.
- Estimating test effort with the user stories.
- Planning test levels and test activities across iterations.

### Iteration Planning

Iteration planning focuses on the scope of a single iteration. The team selects user stories based on priority and capacity, performs detailed analysis, and defines tasks.

### Tester roles in iteration planning include:

- Analyzing user stories risks.
- Determining story testability.
- Creating acceptance tests.
- Defining and estimating testing tasks.
- Identifying functional and non-functional testing needs.
- Supporting test automation for the selected stories.

### Planning Considerations and Adaptability

Release and iteration plans may change due to internal (velocity, delivery capacity) or external (market changes, competition) factors. Agile testers must adapt quickly while maintaining a clear understanding of test objectives and strategy. Testing must be planned in parallel with development.

### Test planning aspects include:

- Scope and extent of testing, including goals and reasons for these decision.
- Roles and responsibilities in test activities.
- Test environments and data requirements.
- Test schedules, dependencies, and frequency.
- Risks to address and their impact on planning.

In addition, the larger team estimation effort should include consideration of the time and effort needed to complete the required testing activities.