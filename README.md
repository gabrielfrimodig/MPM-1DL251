# Exam notes

The topics of the exam will be:

* *Software Processes* (Lecture 1)
* *Requirements Engineering* (Lecture 2)
* *Architectural Design* (Lecutre 4)
* *Inspection* (Lecture 6, aka "Maintenance")
* *Group dynamics* (Lecture 9, aka "Project management")

## Lecture 1 & 2

**Define software engineering, explain the engineering view on SE and what are the relevant constrains.** \
*Software Engineering is a great combination between artistry and engineering* - Bill Gates

Software Engineering is about **processes** to create software. Concerned with theories, methods and tools to create software. \
Possible constrains are often time, money or the organization. \
SE differs from other form of engineering in that every project  is mostly new, it is *invisible*, tha complexity implies lack of physical boundaries and the use of legacy systems.

**Define the concept of process-based quality. Explain the advantages and disadvantages.** \
![Process-based quality](/images/processbased.png "Process-based quality")
Instead of measuring the quality of the process, we measure the quality of the product. It's based on the idea that a good result means a good process. If the end product is good then we standardize that process. \
The problem with this approach is that a bad process could (by luck) genereate a good result. And by this approach we would then standardize a bad process. It's otherwise easy to understand and does in mostly work.

**List the 4 metrics used to measure the quality of a product, explain how we can actually measure them using a process.**
| **Metrics**                                    | **Measure**                                                   |
|------------------------------------------------|---------------------------------------------------------------|
| **Acceptable** - usable, learnable, compatible | **People actually follow it** - acceptable, usable, learnable |
| **Dependable** - safe, reliable, secure        | **Manageable** - Visible, robust to problems                  |
| **Efficient** - response time, memory use      | **It delivers** - efficient, in time, acceptable              |
| **Maintainable** - documented, structured      | **Supportable** - documented, structured                      |

**Identify the differences between plan driven and incremental processes.** \
**Plan driven processes** - are more structured and have a more detailed plan. All of the process activities are planned in advance. \
**Incremental processes** - are more flexible and can be changed during the process. Manage chaning (understanding of customer requirements). Where you can change the plan during the process according to the customer requirements.

**Describe, sketch a working diagram and explain both, when and how, the 4 main software process activities are done on the following processes. Explain the advantages and disadvantages of each one:**

* **Waterfall model** \
![Waterfall model](/images/waterfall.png "Waterfall model") \
Because of the cascade from one phase to another, this model is known as the *waterfall model*, which is an example of a plan-driven process. In principle, you must plan and schedule all of the process activities before starting work on them. The following phase should not start until the previous phase has finished. \
The waterfall model should only be used when the requirements are well understood and unlikely to change readically during system development. \
**Advantages** - Well suited to smaller projects with deliverable that are easy to define from the start. It can provide more predictable end result for budget, timeline and scope. \
**Disadvantages** - The major problem is the infexible partitioning of the project into distinct stages. Commitments must be made at an early stage in the process, which makes it difficult to respond to changing costumer requirements. \
The waterfall methodology focuses very little on the end user or client involved with the project.
* **V-Model** \
![V-model](/images/vmodel.png "V-model") \
The *V-model* is a verification and validation model used in a software development life cycle where each level of development life-cycle is verified before moving to the next level. It is a sequential execution of the process in which each phase is completed before the next phase can begin. \
**Advantages** - It is simple and easy to use. Since the testing starts as soon as the project requirements are written, it increases the sucess rate of the product and possible saves a lot of time. It's easy to manage and each phase are well defined. \
**Disadvantages** - Sequential processes are rigid and not suitable if the requirements are not consistent. The client can only see the final product and not the intermediate modules of product being deisnged, since software is developed during the implementation phase meaning no early prototypes of the software are being produced. Not suitable for complex project and are in general a inflexible model. 

    Suitable for smaller or medium size projects where the requirements are clearly defined and fixed.
* **Incremental development** \
![Incremental](/images/incremental.png "Incremental") \
*Incremental development* is based on the idea of developing an initial implementa-
tion, exposing this to user comment and evolving it through several versions until an
adequate system has been developed. The process is divided into various builds. Cycles are divided up into smaller, more easily managed modules. A working version of software is produced during the first module, so you have working software early during the software life cycle. \
It is better than a waterfall approach for most business, e-commerce, and
personal systems. Incremental development reflects the way that we solve prob-
lems. We rarely work out a complete problem solution in advance but move toward
a solution in a series of steps, backtracking when we realize that we have made a
mistake.\
**Advantages** – It quickly generate a working software module and is highly flexible (less costly to change scope and requirements). Easy to test and debug during a smaller iteration. Customer can respond to each built. \
**Disadvantages** – Needs good planning and design. Needs a clear and complete definition of the whole system before it can be broken down and built incrementally. Total cost tends to be high.

    Used when requirements of the complete system are clearly defined and understood. At least major requirements. Else if we need a early market release.
* **Reuse-based development** \
![Reuse-based](/images/reusebased.png "Reuse-based") \
In which software is redesigned through creating a sequence of prototypes known as models. Every system is derived from the previous one with constant series of defined rules. The reuse model has 4 fundamental steps: to identify components of old system that are most suitable for reuse, to understand all system components, to modify old system components to achieve new requirements and to integrate all of modified parts into new system. \
**Advantages** – It may reduce the total cost of software development with a very low risk factor. It  potentially saves a lot of time and got a high efficient. \
**Disadvantages** – Compromises in requirements may lead to a system that does not fulfill requirements of user. And sometimes using old system component, that is not compatible with new version of component, this may lead to an impact on system evolution.

**Define user requirements** \
Requirements are about **what**, not how. Requirements set by the end user.

**Define system requirements. Compare user requirements and system requirements in terms of what they describe, how they are created and how they are used.** \
User requirements is by its nature very abstract, as it is all about what the end user wants.
System requirements describe what the software must do.
| **User**         | **System**                              |
|------------------|-----------------------------------------|
| Abstract         | More concrete, detailed                 |
| Natural language | Natural + Formal language               |
| What user wants  | What system provides                    |
|                  | Used as contract or product description |

**Define functional requirements.** \
Functional requirements is a description of the service that the software must offer. It describes a software system or its component. Functional software requirements help you to capture the intended behavior of the system. \
For example: “*The software system should be integrated with banking API*” \
**Complete:** All desired functionality is covered. \
**Consistent:** They do not contradict each other.

**Define non-functional requirements. Compare functional requirements and non-functional requirements in terms of what they describe and how they are used.** \
System requirements can be divided into two parts: functional och non-functional. \
**Functional requirements** - are requirements that the end user specifically demands as basic facilities that the system must offer.  Something that must be included in the final product. \
**Non-functional requirements** - is the quality constraints that the system must satisfy according to the project contract. Could be issues like security, scalability, performance etc. Constrains on the system. These are just as important as the functional requirements. 

All non-functional requirements must be measurable.

**Formulate functional and non-functional requirements from a brief description of a product.** \
For example: *email-service*. \
**Functional requirements** - authentication of a user when he/she tries to log into the system. System shutdown in case of a cyber attack. \
**Non-functional requirements** - each login request should be processed within 10 seconds. Emails should be sent with a latency of no greater than 12 hours.

**Describe, sketch a working diagram of the spiral view of process, emphasising the actors responsible for each process and their main responsabilities.** \
![Spiral](/images/spiral.png "Spiral") \
We start in the middle and work in circles.

**Define requirements elicitation, explain its use in the software engineering process and the role of all actors involved.** \
![Requirements Elicitation](/images/requirementselicitation.png "Requirements Elicitation") \

1. **Requirements discovery** – Interacting with the stakeholders.
2. **Requirements classification and organization** – Takes the unstructured collection of requirements, groups related requirements, and organizes them into coherent clusters.
3. **Requirements prioritization and negotiation** - This activity is concerned with prioritizing requirements and finding and resolving requirements conflicts through negotiation.
4. **Requirements specification** - The requirements (formal and informal) are documented and input into the next round of the spiral.

**Define requirements specification, explain its use in the software engineering process and the role of all actors involved.** \
It is the process of writing down the user and system requirements in a requirements document. Which should be clear, unambiguous, easy to understand, complete and consistent. It should describe the both the functional and non-functional requirements so that the end user can understand it. Should not include details of the system architecture or design. It is and expanded version of the user requirements that are used by SE as the starting point for the system design.

**Formulate a well structured user stories as a use case using the natural language and UML.** \
TODO

**Define requirements validation, explain its use in the software engineering process and the role of all actors involved.** \
![Requirements validation](/images/validation.png "Requirements validation") \
Requirements validation is the process of checking that requirements actually define the system that the customer really wants. It overlaps with analysis as it is concerned with finding problems with the requirements. This process is important as errors in the requirements can lead to a system that does not meet the customer’s needs. \
During the requirements validation process, different types of checks should be carried out.

1. *Validuty checks* - checks that the requirements are consistent with each other and with the system architecture. A user may think that a system is needed to perfrom certain functions, but analysis may identify addtional or different functions that are required.
2. *Consistency checks* - Requirements in the document should not conflict. Meaning no contradictory constraints or different descriptions of the system functions.
3. *Completeness checks* - The requirements document should include requirements that define all functions and the constraints intended by the system user.
4. *Realsism checks* - Using knowledge of existing technology, the requirements should be checked to ensure that they can actually be implemented.
5. *Verifiability* - Contracts between costumer and contractor should always be verifiable. In practice, write a set of tests that can demonstrate that the delivered system meet the specified requirements.

**Define requirements verification, explain its use in the software engineering process and the role of all actors involved.** \

**List the desired characteristics of system requirements. Explain how we can actually measure them.** \
System requirements are more detailed descriptions of the software system's functions, services and operational constraints. The system requirements document should define exactly what is to be implemented. It may be part of the contract between the system buyer and the software developers.

**Compare user stories and tasks in agile methodologies.** \
User story is smallest unit of work in an agile framework. It is a short description of a feature told from the perspective of the person who desires the new capability, usually a user or customer of the system. It should be written in the form of a sentence or two of plain English. \
Tasks decide which specific steps needs to be completed and who is responsible for each of them.

## Lecture 4

**Define software design.** \
A software design is a description of the structure of the software to be implemented, the data models and structures used by the system, the interfaces between system components and, sometimes, the algorithms used.

**Define system design. Compare software design and system design in terms of how the programs are composed.** \

**Describe the model for design process. Explain the function of the following activities in the context of software specification: design inputs, design activities, design outputs.** \

**Describe, sketch a working diagram and classify the architectural patterns as physical vs. logical. Compare the advantages and disadvantages between systems:**

* **Client-server**
* **Master-slave**
* **Distributed component**
* **Layered model**
* **Model-view-controller**

**Describe the N-tier architectural model. Explain the differences between a thin and fat client version.** \

## Lecture 6

**Define code reviews. Explain why they are an important inspection tool.** \
General definition: somebody other than the author comments on program code. \
It’s important since reduction of defect rates, cheaper bug fixes, increase maintainability (clean code preemptively).

**Describe and classify the following review processes based on how formal they are. Compare the advantages and disadvantages between processes:**

* **Pair programming** \
  **How**: Code review happens naturally, as the other pair member reads what is written. \
  **Advantages**: Everything is read by 2 people. \
  **Disadvantages**: No benefit of distance, expansive.
* **Over-the-shoulder** \
  **How**: One programmer presents their work to a reviewer. The programmer is at the keyboard and walks the reviewer through the code.\
  **Advantages**: Light-weight, can be used selectively, explanations are readily available. \
  **Disadvantages**: Little time for reflection, easy to over-explain, coverage not guaranteed.
* **Peer review** \
  **How**: The reviewer inspects a chunk of source code of the programmer, and comments on it. \
  **Advantages**: Gives time for reflection, can be on demand, highlights code documentation issues. \
  **Disadvantages**: Can be seen as adversarial.
* **Pre-checking** \
  **How**: Every check-in is inspected by the owner of the module before being accepted. Checked with an expert. \
  **Advantages**: Everything is inspected, check-in message gives context, knowledgeable reviewer, frequent reviews. \
  **Disadvantages**: Time consumption, legacy, tools needed.
* **Formal meeting** \
  **How**: Several reviewers and programmers sit together for a meeting to discuss previously inspected code. \
  **Advantages**: Many eyes on the code, can handle large change sets, observer friendly. \
  **Disadvantages**: Schedule meetings is hard/expensive, group dynamics and ego concerns.

**Describe how the inspection process works. Explain what are different activities and who is responsible for them before, during and after the meeting. Explain the advantages and disadvantages of the process.** \

**Define the concept of legacy system.** \
Legacy systems are old systems that are still useful and are sometimes critical to business operation. They may be implemented using outdated languages and technology or may use other systems that are expensive to maintain. Often their structure has been degraded by change and documentation is missing or out of date. Nevertheless, it may not be cost effective to replace these systems. They may only be used at certain times of the year or it may be too risky to replace them because the specification has been lost.

**Enumerate the two key metrics we use to decide if to scrap, keep or refactor legacy systems.** \
Business value and System quality

**Describe and sketch a diagram how the two metrics are used to inform the decision of scraping, keeping or refactoring legacy systems.** \
![Business & System Quality](/images/legacy.png "Business & System Quality") \
**Low quality, low business value**: Keeping these systems in operation will be expensive and the rate of the return to the business will be fairly small. These systems should be scrapped. \
**Low quality, high business value**: These systems are making an important business contribution so they cannot be scrapped. However, their low quality means that it is expensive to maintain them. These systems should be reengineered to improve their quality. They may be replaced, if a suitable off-the-shelf system is available. \
**High quality, low business value**: These are systems that don’t contribute much to the business but which may not be very expensive to maintain. It is not worth replacing these systems so normal system maintenance may be continued if expensive changes are not required and the system hardware remains in use. If expensive changes become necessary, the software should be scrapped. \
**High quality, high business value**: These system have to be kept in operation. However, their high quality means that you don’t have to invest in transformation or system replacement. Normal system maintenance should be continued.
## Lecture 9

* Define cost model.
* Explain what are the aspects that can influence the development cost of a product in the following models:
  * Budget-limited model
  * Plan-based model
  * Algorithmic cost models
* Define group dynamics and why they are important for project management.
* Describe the Tuckman's stages of group development and sketch a working diagram emphasising how we can influence each stage.
* Describe the GRIP model.
* Assess and compare how a development team is performing using group dynamics theories.
* Evaluate your own group's hazards, strengths, weakness and performance using group dynamics theories.

# Reading

Software engineering (Ninth Edition) - Ian Sommerville

| **Lecture** | **Reading**            | **Important sections**                                                          |
|-------------|------------------------|---------------------------------------------------------------------------------|
|      1      | 1.1-1.2, 2.1, 2.2.3    | 2.1.1, 2.1.2, 2.2.3                                                             |
|      2      | 2.2.1, 4, 10.3         | 2.2.1, 4-in, 4.1-4.3-in, 4.3.1, 4.5-4.7                                         |
|      4      | 2.1.3, 2.2.2, 6, 16-18 | 2.2.3-Reuse oriented, 2.2.2, 6-Intro, 6.3, 17.2, 18-Intro, 18.2, 18.3.2-18.3.3 |
|      6      | 9, 24-25               | 9.3-9.4, 25.3, 24-intro, 24.1, 24.4                                             |
