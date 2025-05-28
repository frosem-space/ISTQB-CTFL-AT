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

Testers actively participate in all stages, including:

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

In Agile, requirements are captured as user stories. These are created collaboratively by developers, testers, and business representatives.

### Key Concepts
- User stories cover both functional and non-functional aspects.
- Acceptance criteria are essential and must be defined together.
- Testers contribute by refining user stories, identifying gaps, and confirming testability.

### Techniques
- **Brainstorming and mind mapping** help in collaborative story creation.
- **INVEST** criteria define quality user stories:
  - Independent
  - Negotiable
  - Valuable
  - Estimable
  - Small
  - Testable

### 3C Model
- **Card**: Describes the story and key information.
- **Conversation**: Facilitates shared understanding.
- **Confirmation**: Validates completion through acceptance tests.

Documentation should be minimal but sufficient for clarity.

## 1.2.3 Retrospectives

Retrospectives are held at the end of each iteration to assess what worked, what didn’t, and what to improve.

### Purpose and Scope
- Topics include team dynamics, tools, processes, and relationships.
- Aim to support continual improvement in a trusted environment.

### Tester Involvement
- Testers offer input from a unique perspective.
- Retrospectives can target test-related improvements (e.g., test quality, coverage).

Changes should be incremental to allow sustainable progress.

## 1.2.4 Continuous Integration

Continuous integration ensures that software is integrated, built, and tested frequently—often multiple times a day.

### Key Activities
- Static code analysis
- Compilation
- Unit and integration testing
- Deployment to test environments
- Automated reporting (dashboards, emails)

### Benefits
- Early detection of integration issues
- Rapid feedback on quality
- Consistent availability of a testable product
- Reduced regression risks
- Transparent progress

### Challenges
- Requires robust tools and infrastructure
- High initial investment in test automation
- Risks of relying too heavily on unit tests

Continuous integration supports frequent delivery and ongoing quality control.

## 1.2.5 Release and Iteration Planning

Planning in Agile includes both **release planning** (long-term) and **iteration planning** (short-term).

### Release Planning
- Focuses on product vision and backlog prioritization.
- Testers contribute by:
  - Defining testable stories and acceptance criteria
  - Analyzing risks and estimating test effort
  - Determining test levels and planning test activities

### Iteration Planning
- Focuses on selecting and detailing stories for the next sprint.
- Testers contribute by:
  - Analyzing risk and testability of stories
  - Creating acceptance tests and test tasks
  - Estimating effort and supporting automation

### Planning Considerations
- Scope, test environment, data needs
- Task dependencies and sequencing
- Risk-driven prioritization

Plans can change due to internal (velocity, technical issues) or external (market shifts) factors. Testers must adapt while maintaining quality planning and documentation.
