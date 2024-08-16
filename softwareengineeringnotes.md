# Software Engineering

## General Principles
- Design is pivotal.
- Software should exhibit high quality and be maintainable.
- Understand the problem before creating a solution.
- Seminal Definition: Software engineering involves the use of sound engineering principles to develop reliable, efficient, and economical software for real machines.

## IEEE Definition
- Application of a systematic, disciplined, quantifiable approach to software development, operation, and maintenance.
- Study of these approaches.

## Framework Activities
- Communication
- Planning
- Modeling (requirements analysis, design)
- Construction (code generation, testing)
- Deployment

## Umbrella Activities
- Project tracking and control
- Risk management
- Quality assurance
- Technical reviews
- Measurement
- Configuration management
- Reusability management
- Work product preparation and production

## Problem Understanding
- Identify stakeholders.
- Determine unknowns.
- Define data, functions, and features.
- Compartmentalize problems for easier understanding.
- Create analysis models and graphical representations if possible.
- Draw on past experiences with similar problems.

## Hooker’s Principles
- The reason it all exists.
- Keep it simple.
- Maintain the vision.
- Consider future needs.
- Plan for reuse.
- Think critically.

## Process Models
- Linear Process Flow: Sequential phases (Communication -> Planning -> Modeling -> Construction -> Deployment).
- Interactive Process Flow: Iterative back to previous phases.
- Evolutionary Process Flow: Cycles through phases repeatedly.
- Parallel Process Flow: Overlapping activities.

## Task Sets
- Define tasks to accomplish objectives.
- Identify work products.
- Apply quality assurance filters.

## Process Patterns
- Stage Patterns: Problems within a framework activity.
- Task Patterns: Problems with a software engineering action or work task.
- Phase Patterns: Sequence of framework activities, iterative in nature.

## Process Assessment and Improvement
- SCAMPI: Five-phase assessment model (initiating, diagnosing, establishing, acting, learning).
- CBA IPI: Diagnostic technique for assessing software organization maturity.
- SPICE: ISO/IEC15504 standard for software process assessment.
- ISO 9001:2000: Generic standard for quality improvement.

## Software Development Models
### Waterfall Model: Linear, sequential phases.
### V-Model: Validation and verification at each development stage.
### Incremental Model: Multiple development cycles with incremental improvements.
### Evolutionary Models:
- Prototyping: Building prototypes to refine requirements.
- Spiral: Combining iterative development with systematic aspects.
- Concurrent: Simultaneous development activities.

## Additional Process Models
- Component-Based Development: Emphasis on reuse.
- Formal Methods: Mathematical specification of requirements.
- AOSD: Aspect-Oriented Software Development for modular concerns.
- Unified Process (UP): Use-case driven, architecture-centric, iterative.

## Agile Development
### Agility Principles:
- Respond to change.
- Effective communication.
- Customer collaboration.
- Self-organizing teams.
- Rapid, incremental delivery.
- Emphasis on working software.

## Extreme Programming (XP)
- Planning: User stories and delivery dates.
- Design: KISS principle, CRC cards, spike solutions, refactoring.
- Coding: Unit tests, pair programming.
- Testing: Daily unit tests, customer-defined acceptance tests.

## Industrial XP (IXP)
### Expanded roles and technical practices:
- Readiness assessment
- Project community
- Project chartering
- Test-driven management
- Retrospectives
- Continuous learning

## Scrum
- Partitioned development work.
- Ongoing testing and documentation.
- Iterative "sprints."
- Short, frequent meetings.
- Customer demos with time-box allocation.

## DevOps
- Emphasizes collaboration and communication among software developers and IT professionals.
- Automation of software delivery and infrastructure changes.

## Requirements Engineering
- Inception: Basic problem understanding and stakeholder identification.
- Elicitation: Gathering requirements from stakeholders.
- Elaboration: Creating an analysis model for data, function, and behavioral requirements.
- Negotiation: Agreeing on a realistic deliverable system.
- Specification: Documenting requirements (models, scenarios, prototypes).
- Validation: Reviewing requirements for errors, clarifications, and consistency.

## Use-Case Development
- Identify main tasks and functions.
- Determine system information required by actors.
- Define success scenarios and failure conditions.
- Use UML diagrams for visual representation.
- Review and refine primary scenarios.

## OOP Concepts
- Class: Blueprint with functions and abilities.
- Inheritance: Abstract representation of objects.
- Encapsulation: Combining data and operations in one class/object.
- Polymorphism: Different interpretations of a message by different classes/objects.

## Class-Based Modeling
- Represents objects, operations, relationships, and collaborations.
- Generalization: Inheritance relationships.
- Association: Usage relationships (aggregation, composition, dependency).

## CRC Models
- Entity Classes: Business classes extracted from the problem statement.
- Boundary Classes: Interface with the user.
- Controller Classes: Manage units of work from start to finish.

## Responsibilities
### System intelligence should be distributed across classes to best address the needs of the problem.
### System intelligence is an assumption.
### Each responsibility should be stated as generally as possible.
### Information and the behavior related to it should reside within the same class.
- Data + Behavior = encapsulation.
### Information about one thing should be localized with a single class, not distributed across multiple classes.
### Responsibilities should be shared among related classes, when appropriate.

## Collaborations
### Classes fulfill their responsibilities in one of two ways:
- A class can use its own operations to manipulate its own attributes, thereby fulfilling a particular responsibility.
- A class can collaborate with other classes.
### Collaborations identify relationships between classes.
### Collaborations are identified by determining whether a class can fulfill each responsibility itself.
### Three different generic relationships between classes [WIR90]:
- is-part-of relationship
- has-knowledge-of relationship
- depends-upon relationship

## Reviewing the CRC Model
### All participants in the review (of the CRC model) are given a subset of the CRC model index cards.
### Cards that collaborate should be separated (i.e., no reviewer should have two cards that collaborate).
### All use-case scenarios (and corresponding use-case diagrams) should be organized into categories.
### The review leader reads the use-case deliberately.
### As the review leader comes to a named object, she passes a token to the person holding the corresponding class index card.
### When the token is passed, the holder of the class card is asked to describe the responsibilities noted on the card.
### The group determines whether one (or more) of the responsibilities satisfies the use-case requirement.
### If the responsibilities and collaborations noted on the index cards cannot accommodate the use-case, modifications are made to the cards.
- This may include the definition of new classes (and corresponding CRC index cards) or the specification of new or revised responsibilities or collaborations on existing cards.

## Analysis Packages
### Various elements of the analysis model (e.g., use-cases, analysis classes) are categorized in a manner that packages them as a grouping.
### The plus sign preceding the analysis class name in each package indicates that the classes have public visibility and are therefore accessible from other packages.
### Other symbols can precede an element within a package:
- A minus sign indicates that an element is hidden from all other packages.
- A # symbol indicates that an element is accessible only to packages contained within a given package.
