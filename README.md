# Exam notes

The topics of the exam will be:

* *Software Processes* (Lecture 1)
* *Requirements Engineering* (Lecture 2)
* *Architectural Design* (Lecutre 4)
* *Inspection* (Lecture 6, aka "Maintenance")
* *Group dynamics* (Lecture 9, aka "Project management")

## Lecture 1 & 2

### **Define software engineering, explain the engineering view on SE and what are the relevant constrains**

Software Engineering is about *processes* to create software. Concerned with theories, methods and tools to create software. Possible constrains are often time, money or the organization. \
SE differs from other form of engineering in that every project  is mostly new, it is *invisible*, tha complexity implies lack of physical boundaries and the use of legacy systems.

### **Define the concept of process-based quality. Explain the advantages and disadvantages**

![Process-based quality](/images/processbased.png "Process-based quality")
Instead of measuring the quality of the process, we measure the quality of the product. It's based on the idea that a good result means a good process. If the end product is good then we standardize that process. \
The problem with this approach is that a bad process could (by luck) genereate a good result. And by this approach we would then standardize a bad process. It's otherwise easy to understand and does in work in many cases.

### **List the 4 metrics used to measure the quality of a product, explain how we can actually measure them using a process**

| **Metrics**                                    | **Measure**                                                   |
|------------------------------------------------|---------------------------------------------------------------|
| **Acceptable** - usable, learnable, compatible | **People actually follow it** - acceptable, usable, learnable |
| **Dependable** - safe, reliable, secure        | **Manageable** - Visible, robust to problems                  |
| **Efficient** - response time, memory use      | **It delivers** - efficient, in time, acceptable              |
| **Maintainable** - documented, structured      | **Supportable** - documented, structured                      |

### **Identify the differences between plan driven and incremental processes**

**Plan driven processes** - are more structured and have a more detailed plan. All of the process activities are planned in advance. \
**Incremental processes** - are more flexible and can be changed during the process. Manage chaning (understanding of customer requirements). Where you can change the plan during the process according to the customer requirements.

### **Describe, sketch a working diagram and explain both, when and how, the 4 main software process activities are done on the following processes. Explain the advantages and disadvantages of each one:**

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
Suitable for smaller or medium size projects where the requirements are clearly defined and fixed. \
**Advantages** - It is simple and easy to use. Since the testing starts as soon as the project requirements are written, it increases the sucess rate of the product and possible saves a lot of time. It's easy to manage and each phase are well defined. \
**Disadvantages** - Sequential processes are rigid and not suitable if the requirements are not consistent. The client can only see the final product and not the intermediate modules of product being deisnged, since software is developed during the implementation phase meaning no early prototypes of the software are being produced. Not suitable for complex project and are in general a inflexible model.

* **Incremental development** \
![Incremental](/images/incremental.png "Incremental") \
*Incremental development* is based on the idea of developing an initial implementation, exposing this to user comment and evolving it through several versions until an
adequate system has been developed. The process is divided into various builds. Cycles are divided up into smaller, more easily managed modules. A working version of software is produced during the first module, so you have working software early during the software life cycle. \
It is better than a waterfall approach for most business, e-commerce, and personal systems. Incremental development reflects the way that we solve problems. We rarely work out a complete problem solution in advance but move toward a solution in a series of steps, backtracking when we realize that we have made a mistake. \
Used when requirements of the complete system are clearly defined and understood. At least major requirements. Else if we need a early market release. \
**Advantages** – It quickly generate a working software module and is highly flexible (less costly to change scope and requirements). Easy to test and debug during a smaller iteration. Customer can respond to each built. \
**Disadvantages** – Needs good planning and design. Needs a clear and complete definition of the whole system before it can be broken down and built incrementally. Total cost tends to be high. \
From a management perspective, the incremental approach has two problems:
  1. The process is not visible. Managers need regular deliverables to measure
progress. If systems are developed quickly, it is not cost-effective to produce
documents that reflect every version of the system.
  1. System structure tends to degrade as new increments are added. Unless time and
money is spent on refactoring to improve the software, regular change tends to
corrupt its structure. Incorporating further software changes becomes increas-
ingly difficult and costly.

* **Reuse-based development** \
![Reuse-based](/images/reusebased.png "Reuse-based") \
In the majority of software projects, there is some software reuse. Often times the  software is redesigned through creating a sequence of prototypes known as models. Every system is derived from the previous one with constant series of defined rules. The reuse model has 4 fundamental steps: to identify components of old system that are most suitable for reuse, to understand all system components, to modify old system components to achieve new requirements and to integrate all of modified parts into new system. \
**Advantages** – It may reduce the total cost of software development with a very low risk factor. It  potentially saves a lot of time and got a high efficient. It usually also leads to faster delivery of the software. \
**Disadvantages** – Compromises in requirements may lead to a system that does not fulfill requirements of user. And sometimes using old system component, that is not compatible with new version of component, this may lead to an impact on system evolution.

### **Define user requirements**

User requirements is by its nature very abstract, as it is all about what the end user wants. It is statements (in a natural language) of what services the system is expected to provide to the end users and the constraints under which it must operate. The user requirements may vary from broad statements of the system features required to detailed, precise descriptions of the system functionality.

### **Define system requirements. Compare user requirements and system requirements in terms of what they describe, how they are created and how they are used**

System requirements are more detailed descriptions of the software system’s functions, services, and operational constraints. The system requirements document should define exactly what is to be implemented. It may be part of the contract between the system buyer and the software developers.

System requirements describe what the software must do.
| **User**         | **System**                              |
|------------------|-----------------------------------------|
| Abstract         | More concrete, detailed                 |
| Natural language | Natural + Formal language               |
| What user wants  | What system provides                    |
|                  | Used as contract or product description |

The readers of the user requirements are not usually concerned with how the system will be implemented and the readers of the system requirements need to know more precisely what the system will do.

System requirements are classified as functional and non-functional requirements.

### **Define functional requirements**

Functional requirements is a description of the service that the software must offer and how the system should behave in particular situations. It describes a software system or its component. Functional software requirements help you to capture the intended behavior of the system. \
For example: “*The software system should be integrated with banking API*” \
**Complete:** All desired functionality is covered. \
**Consistent:** They do not contradict each other.

### **Define non-functional requirements. Compare functional requirements and non-functional requirements in terms of what they describe and how they are used**

Non-functional requirements are constraints on the services or functions offered by the system. It includes timing constraints, different constraints on the development process and constraints imposed by standards. Its often applied to the system as a whole rather than individual system features or services. Non-functional arguments must always be measurable. Could be issues like security, scalability, performance etc. Constrains on the system. These are just as important as the functional requirements. Compare to functional: see question above.

Non-functional requirements can be divided into subcategories.

![Non-functional Requirements](/images/non-func.png "Non-functional Requirements") \

### **Formulate functional and non-functional requirements from a brief description of a product**

For example: *email-service*. \
**Functional requirements**: Authentication of a user when he/she tries to log into the system. System shutdown in case of a cyber attack. \
**Non-functional requirements**: Each login request should be processed within 10 seconds. Emails should be sent with a latency of no greater than 12 hours.

### **Describe, sketch a working diagram of the spiral view of process, emphasising the actors responsible for each process and their main responsabilities**

Requirements engineering processes may include four different high-level activities. These focus on assessing if the system is useful to the business (feasibility study), discovering requirements (elicitation and analysis), converting these requirements into some standard form (specification), and checking that the requirements actually define the system that the customer wants (validation). \
The activities are organized as an iterative process around a spiral, with the output being a system requirements document. The amount of time and effort devoted to each activity in each iteration depends on the stage of the overall process and the type of system being developed. Early in the process, most effort will be spent on understanding high-level business and non-functional requirements, and the user requirements for the system. Later in the process, in the outer rings of the spiral, more effort will be devoted to eliciting and understanding the detailed system requirements. This spiral model accommodates approaches to development where the requirements are developed to different levels of detail. The number of iterations around the spiral can vary so the spiral can be exited after some or all of the user requirements have been elicited. Agile development can be used instead of prototyping so that the requirements and the system implementation are developed together.

![Spiral](/images/spiral.png "Spiral")

### **Define requirements elicitation, explain its use in the software engineering process and the role of all actors involved**

The aims of the requirements elicitation process are to understand the work that stakeholders do and how they might use a new system to help support that work. During requirements elicitation, software engineers work with stakeholders to find out about the application domain, work activities, the services and system features that stakeholders want, the required performance of the system, hardware constraints, and so on. \
Requirements elicitation is the process of gathering information about the required system and existing systems, and distilling the user and system requirements from this information. Source of information includes documentation, system stakeholders, system users and other systems.

![Requirements Elicitation](/images/requirementselicitation.png "Requirements Elicitation")

1. **Requirements discovery**: This is the process of interacting with stakeholders of the system to discover their requirements. Domain requirements from stakeholders and documentation are also discovered during this activity.
2. **Requirements classification and organization**: Takes the unstructured collection of requirements, groups related requirements, and organizes them into coherent clusters. The most common way of grouping requirements is to use a model of the system architecture to identify sub-systems and to associate requirements with each sub-system.
3. **Requirements prioritization and negotiation**: When we have multiple stakeholders involved there sure will be conflicts. This activity is concerned with prioritizing requirements and finding and resolving requirements conflicts through negotiation.
4. **Requirements specification**: The requirements (formal and informal) are documented and input into the next round of the spiral.

### **Define requirements specification, explain its use in the software engineering process and the role of all actors involved**

It is the process of writing down the user and system requirements in a requirements document. The requirements document is an official statemnt of what the sytem developers should implement. It includes both user requirements for a system and a detailed specification of the system requirements. Which should be clear, unambiguous, easy to understand, complete and consistent. It should describe the both the functional and non-functional requirements so that the end user can understand it. Should not include details of the system architecture or design. It is and expanded version of the user requirements that are used by SE as the starting point for the system design.

System requirements should be written in natural language but other notations based on forms, graphical system models or mathematical system models can also be used.

![Users of a requirements document](/images/users-of-requirements.png "Users of a requirements document")

### **Formulate a well structured user stories as a use case using the natural language and UML**

Use cases is a fundamental feature of the unified modeling language. In their simplest form, a use case identifies the actors involved in an interaction and names the type of interaction. This is then supplemented by additional information describing the interaction with the system. The additional information may be a textual description or one or more graphical models such as UML sequence or state charts. \
Use cases are documented using a high-level use case diagram. The set of use cases represents all of the possible interactions that will be described in the system requirements. Actors in the process, who may be human or other systems, are represented as stick figures.

**Example**: *The system should be able to show a brown 5x5 board that outlines the playing field for both players from the moment that a gaming session is initialized until the moment that a gaming session has ended.*

![UML](/images/umlex.png "UML")

### **Define requirements validation, explain its use in the software engineering process and the role of all actors involved.**

Validation is the process of evaluating software during or at the end of the development process to determine whether it satisfies specified requirements. \
It ask: *will the product satisfy the costumer needs? Are we building the right product? Is the product usable?*

![Requirements validation](/images/validation.png "Requirements validation") \
Requirements validation is the process of checking that requirements actually define the system that the customer really wants. It overlaps with analysis as it is concerned with finding problems with the requirements. This process is important as errors in the requirements can lead to a system that does not meet the customer’s needs. \
During the requirements validation process, different types of checks should be carried out. Validation may also involve checking processes, such as inspections and reviews, at each stage of the software process from user requirements definition to program development.

1. **Validuty checks**: Checks that the requirements are consistent with each other and with the system architecture. A user may think that a system is needed to perfrom certain functions, but analysis may identify addtional or different functions that are required.
2. **Consistency checks**: Requirements in the document should not conflict. Meaning no contradictory constraints or different descriptions of the system functions.
3. **Completeness checks**: The requirements document should include requirements that define all functions and the constraints intended by the system user.
4. **Realsism checks**: Using knowledge of existing technology, the requirements should be checked to ensure that they can actually be implemented.
5. **Verifiability**: Contracts between costumer and contractor should always be verifiable. In practice, write a set of tests that can demonstrate that the delivered system meet the specified requirements.

### **Define requirements verification, explain its use in the software engineering process and the role of all actors involved**

Verification is the process of evaluating software to determine whether the products of a given development phase satisfy the conditions imposed at the start of that phase. \
It ask the question: *do we satisfy the requirements? Are we building the product right? Is the contract fulfilled?*

### **List the desired characteristics of system requirements. Explain how we can actually measure them**

System requirements are more detailed descriptions of the software system's functions, services and operational constraints. The system requirements document should define exactly what is to be implemented. It may be part of the contract between the system buyer and the software developers.

Desired characteristics of system requirements: completing the requirements, consistency, correctness, completeness, feasibility, modifiability, non-ambiguity, non-redundancy, non-repudiation, non-triviality, operability, precision, prioritization, realism, testability, traceability, verifiability, verisimilitude, and verisimilitude.

### **Compare user stories and tasks in agile methodologies**

User story is smallest unit of work in an agile framework. It is a short description of a feature told from the perspective of the person who desires the new capability, usually a user or customer of the system. It should be written in the form of a sentence or two of plain English. \
Tasks decide which specific steps needs to be completed and who is responsible for each of them.

User stories are presentation of the user requirement and is written as: **user role** needs to **do something** for **a reason**. It can be presented as UML diagrams.

On the other hand, tasks present incremental change that are being made to system. It is a activity to prepare the change. Can be presented as cards with description on the activity.

## Lecture 4

### **Define software design**

A software design is a description of the structure of the software to be implemented, the data models and structures used by the system, the interfaces between system components and, sometimes, the algorithms used. \
It is the composition of a single program, decomposted into layers and modules and looks at interactiv patterns. \

### **Define system design. Compare software design and system design in terms of how the programs are composed**

System design is the process of designing the elements of a system such as the architecture, modules and components, the different interfaces of those components and the data that goes through that system. This process overlaps significantly with the requirements development process. It involves establishing the overall architecture of the system, identifying the different system components and understanding the relationships between them.

Software design is all about building a design plan that delves into the different elements that make up a system. It shows how they work together to fulfill the system requirements. It concentrates on the system’s implementation, often delving into considerable detail. Software design centers on the selection of algorithms and data structures, as well as the implementation details of every single component.


### **Describe the model for design process. Explain the function of the following activities in the context of software specification: design inputs, design activities, design outputs**

A software design is a description of the structure of the software to be implemented, the data models and structures used by the system, the interfaces between system components and, sometimes, the algorithms used.

![Design process](/images/designprocess.png "Design process") \
The diagram suggests that the stages of the design process are sequential. In fact, design process activities are interleaved. Feedback from one stage to another and consequent design rework is inevitable in all design processes.

**Design inputs** \
Inputs to the system is platform information, requirements specification and data description.

**Design activities** \
The activities in the design process vary, depending on the type of system being developed. For example, real-time systems require timing design but may not include a database so there is no database design involved. The design activities are:

1. *Architectural design*, where you identify the overall structure of the system, the principal components (sometimes called sub-systems or modules), their relationships, and how they are distributed.
2. *Interface design*, where you define the interfaces between system components. This interface specification must be unambiguous. With a precise interface, a component can be used without other components having to know how it is implemented. Once interface specifications are agreed, the components can be designed and developed concurrently.
3. *Component design*, where you take each system component and design how it will operate. This may be a simple statement of the expected functionality to be implemented, with the specific design left to the programmer. Alternatively, it may be a list of changes to be made to a reusable component or a detailed design model. The design model may be used to automatically generate an implementation.
4. *Database design*, where you design the system data structures and how these are to be represented in a database. Again, the work here depends on whether an existing database is to be reused or a new database is to be created.

**Design outputs** \
The output of the design activities will result in system architecture and specification of the system.

### **Describe, sketch a working diagram and classify the architectural patterns as physical vs. logical. Compare the advantages and disadvantages between systems:**

* **Client-server** (physical) \
![Client-server](/images/client-server.png "Client-server") \

|       |                        |
|-------|------------------------|
| **Good:**  | Easy to extend, secure |
| **Issue:** | Bottleneck: network    |


* **Master-slave** (physical) \
![Master-slave](/images/master-slave.png "Master-slave") \

|           |                                                          |
|-----------|----------------------------------------------------------|
| **Good**  | Dedicated processes (slave), Great for real-time systems |
| **Issue** | Not so extensible / secure                               |

* **Distributed component** (physical) \
![Distributed component](/images/distributed.png "Distributed component") \

|          |                                                                                                                                      |
|----------|--------------------------------------------------------------------------------------------------------------------------------------|
| **Good** | Allows system designer to delay decisions on when/how services are provided, Flexible / Scalable / Extensible / Auto-reconfiguration |
| **Bad**  | Complex                                                                                                                              |

* **Layered model** (logical) \
![Layered Model](/images/layered.png "Layered Model") \

|           |                                                                                              |
|-----------|----------------------------------------------------------------------------------------------|
| **Good**  | Used to model interacting subsystems                                                         |
| **Good**  | Organizes system into set of layers: each layer provides only a set of services              |
| **Good**  | Supports reuse: changes in one layer does not affect others, layers can be merged / splitted |
| **Issue** | Too simple                                                                                   |
| **Bad**   | Performance: needs to bypass layers                                                          |

* **Model-view-controller** (logical) \
![Model View Controller](/images/model-view-controller.png "Model View Controller") \

|           |                                                                                                                                            |
|-----------|--------------------------------------------------------------------------------------------------------------------------------------------|
| **Good**  | Separates presentation/interaction/data: data can change independently of its representation, allows presenting same data in multiple ways |
| **Issue** | Too simple: might involve extra coding, requires to adapt the logical architecture                                                         |

### **Describe the N-tier architectural model. Explain the differences between a thin and fat client version**

The N-tier architecture is a client-server architecture in which the presentation tier, application tier, and data tier are each implemented as a separate layer. The N-tier architecture is a client-server architecture in which the presentation tier, application tier, and data tier are each implemented as a separate layer.

A two-tier client–server architecture is the simplest form of client–server architecture. The system is implemented as a single logical server plus an indefinite number of clients that use that server.

![Thin- and fat-client architectural models](/images/thinfat.png "Thin- and fat-client architectural models") \

**Thin-client model:** A thin-client model, where the presentation layer is implemented on the client and all other layers (data management, application processing, and database) are implemented on a server. The client software may be a specially written program on the client to handle presentation. More often, however, a web browser on the client computer is used for presentation of the data. \
The advantage of the thin-client model is that it is simple to manage the clients. This is a major issue if there are a large number of clients, as it may be difficult and expensive to install new software on all of them. If a web browser is used as the client, there is no need to install any software. The disadvantage of the thin-client approach, however is that it may place a heavy processing load on both the server and the network.

**Fat-client model:** A fat-client model, where some or all of the application processing is carried out on the client. Data management and database functions are implemented on the server. \
The fat-client model makes use of available processing power on the computer running the client software, and distributes some or all of the application processing and the presentation to the client. The server is essentially a transaction server that manages all database transactions. Data management is straightforward as there is no need to manage the interaction between the client and the application processing system. Of course, the problem with the fat-client model is that it requires additional system management to deploy and maintain the software on the client computer. An example of a situation in which a fat-client architecture is used is in a bank ATM system, which delivers cash and other banking services to users.
## Lecture 6

### **Define code reviews. Explain why they are an important inspection tool**

General definition: somebody other than the author comments on program code. \
It’s important since reduction of defect rates, cheaper bug fixes, increase maintainability (clean code preemptively).

### **Describe and classify the following review processes based on how formal they are. Compare the advantages and disadvantages between processes:**

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

**From most formal to less complex**: Formal meeting, Client validation, Peer Review. Over-the-shoulder, Pair Programming

### **Describe how the inspection process works. Explain what are different activities and who is responsible for them before, during and after the meeting. Explain the advantages and disadvantages of the process**

Inspections mostly focus on the source code of a system but any readable representation of the software, such as its requirements or a design model, can be inspected. When you inspect a system, you use knowledge of the system, its application domain, and the programming or modeling language to discover errors. 

The goals of inspections are: finding errors, checking adherence to standards, readability, collecting data about common errors.

|          |                                                             |
|----------|-------------------------------------------------------------|
| **Good** | Apply to all documents: no program needed                   |
| **Good** | Quality perspective from the start                          |
| **Bad**  | Do not cover emergent properties:most apply to verification |
| **Bad**  | Added cost early in the process                             |

There are three advantages of software inspection over testing:

1. During testing, errors can mask (hide) other errors. When an error leads to unexpected outputs, you can never be sure if later output anomalies are due to a new error or are side effects of the original error. Because inspection is a static process, you don’t have to be concerned with interactions between errors. Consequently, a single inspection session can discover many errors in a system.
2. Incomplete versions of a system can be inspected without additional costs. If a program is incomplete, then you need to develop specialized test harnesses to test the parts that are available. This obviously adds to the system development costs.
3. As well as searching for program defects, an inspection can also consider broader quality attributes of a program, such as compliance with standards, portability, and maintainability. You can look for inefficiencies, inappropriate algorithms, and poor programming style that could make the system difficult to maintain and update.

![Inspection](/images/inspection.png "Inspection") \

However, inspections cannot replace software testing. Inspections are not good for discovering defects that arise because of unexpected interactions between different parts of a program, timing problems, or problems with system performance. Furthermore, especially in small companies or development groups, it can be difficult and expensive to put together a separate inspection team as all potential members of the team may also be software developers.

### **Define the concept of legacy system**

Legacy systems are old systems that are still useful and are sometimes critical to business operation. They may be implemented using outdated languages and technology or may use other systems that are expensive to maintain. Often their structure has been degraded by change and documentation is missing or out of date. Nevertheless, it may not be cost effective to replace these systems. They may only be used at certain times of the year or it may be too risky to replace them because the specification has been lost.

### **Enumerate the two key metrics we use to decide if to scrap, keep or refactor legacy systems**

Business value and System quality

### **Describe and sketch a diagram how the two metrics are used to inform the decision of scraping, keeping or refactoring legacy systems.**

![Business & System Quality](/images/legacy.png "Business & System Quality") \
**Low quality, low business value**: Keeping these systems in operation will be expensive and the rate of the return to the business will be fairly small. These systems should be scrapped.

**Low quality, high business value**: These systems are making an important business contribution so they cannot be scrapped. However, their low quality means that it is expensive to maintain them. These systems should be reengineered to improve their quality. They may be replaced, if a suitable off-the-shelf system is available.

**High quality, low business value**: These are systems that don’t contribute much to the business but which may not be very expensive to maintain. It is not worth replacing these systems so normal system maintenance may be continued if expensive changes are not required and the system hardware remains in use. If expensive changes become necessary, the software should be scrapped.

**High quality, high business value**: These system have to be kept in operation. However, their high quality means that you don’t have to invest in transformation or system replacement. Normal system maintenance should be continued.

## Lecture 9

### **Define cost model**

Describes the cost of a software system in terms of the resources required to build and maintain it.

### **Explain what are the aspects that can influence the development cost of a product in the following models:**

* **Budget-limited model** \
  We implement as much as the budget allows. Price is fixed. We can only influence the profit. \
  Profit is influenced by: risks (highly), subcontracts (slightly), reusability (slightly). \
  Outcome determined by: requirements, available people, budget, risks, eventual ownership.
  
* **Plan-based model** \
We implement as much as the time allows. **Requirements** are agreed and **we can influence** them. \
Cost is mostly influenced by: salary costs, requirements satisfaction. Possible overhead: facilities, recruitment, support staff, computers, network, etc.

* **Algorithmic cost models** \
Compute project effort based on estimates of product attributes, e.g. size, and process characteristics, such as experience of staff involved. \
Calclulated by: Organizational constant x Project and process x Size

### **Define group dynamics and why they are important for project management**

Team dynamics is a system of behaviors and psychological processes occurring within a team. Group dynamics defines how effective your team is going to be in their work performance and generating new ideas. As a result, it influences the overall project outcome.

An important aspect of effective teamwork entails understanding group dynamics in terms of both team situation and individual temperament.

### **Describe the Tuckman's stages of group development and sketch a working diagram emphasising how we can influence each stage**

![Tuckman's stages](/images/tuckman.png "Tuckman's stages") \
Stages are not linear. Teams can move back and forth between stages based on events influencing the team  (e.g., conflict resolution) and communication strategies.

  1. **Forming** \
The team gets to know each other and make good impression. Good time to create shared expectations, guidelines. It is at this stage boundaries are formed.
  2. **Storming** \
  We learn about each other's motivation. Preliminary boundaries and expectations are challenged. During the brainstorming: ideas are shared, strangths and weakness become apparent and roles start to be determined. \
  Learning how to use the constructive potential of conflict and compromise key to progress.
  3. **Norming** \
  Conflicts have been solved and teammates have proved flexible. Everyone knows its role and works on their part of the project. \
  Problem emerge if: Someone does not understand their role, the team expectation is unclear or the overall goal is unclear. \
  There is a risk to go back to the forming or storming stages. \
  Group cohesion ensures everyone is responsible to the task and to each other.
  4. **Performing** \
  The team has developed a synergy after working togheter long enough. There is **group synergy** and there are **processes** in place.
  5. **Adjourning** \
  Goodbye.


### **Describe the GRIP model**

![GRIP Model](/images/grip.png "GRIP Model") \
This model outlines four interrelated components of highly effective team. \
Each component influences the following (clockwise).

1. **Goal** \
Everyone must understand and be fully committed to the goals and the organization. Individual goals must be aligned to establish: trust, make progress, achieve outcome.
2. **Roles** \
Everyone in the team knows: what part they play, what is expected and how they are going to be held accountable/responsible.
3. **Interpersonal** \
High quality of communication and collaboration: to increase trust \
Sensitivity and flexibility: to deal with conflict, to make progress.
4. **Processes** \
Defines systems for: how decisions are made, how the teams solves problems and addresses conflicts. \
Defined systems and procedures to: completing the project.

**Example** \
Task: *who owns the task?* **(roles)** \
Accountability: *do they have the authority to be held accountable?* **(interpersonal)** \
Success: *do we agree that they are set up for success?* **(goals + roles + interpersonal)** \
Checklist: *do we have a checklist of what needs to happen to accomplish the task?* **(processes)**

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


# Bonus

## Testing

The stages in the testing process are:
1. *Development testing* - The components making up the system are tested by the people developing the system. Each component is tested independently, without the influence of other components.
2. *System testing* - System components are integrated to create a complete system. This process is concerned with finding errors that result from unanticipated interactions between components and component interface problems. It is also concerned with showing that the system meets its functional and non-functional requirements, and testing the emergent system properties.
3. *Acceptance testing* - This is the final stage in the testing process before the system is accepted for operational use. The system is tested with data supplied by the system customer rather than with simulated test data. Acceptance testing may reveal errors and omissions in the system requirements definition, because the real data exercise the system in different ways from the test data. Acceptance testing may also reveal requirements problems where the system’s facilities do
not really meet the user’s needs or the system performance is unacceptable.

![Testing](/images/testing.png "Testing")

###  Requirements engineering

Software specification or requirements engineering is the process of understanding
and defining what services are required from the system and identifying the con-
straints on the system’s operation and development.

There are four main activities in the requirements engineering process:
1. *Feasibility study* - An estimate is made of whether the identified user needs may be satisfied using current software and hardware technologies. The study considers whether the proposed system will be cost-effective from a business point of view and if it can be developed within existing budgetary constraints. A feasibility study should be relatively cheap and quick. The result should inform the decision of whether or not to go ahead with a more detailed analysis.
2. *Requirements elication and analysis* - This is the process of deriving the system requirements through observation of existing systems, discussions with potential users and procurers, task analysis, and so on. This may involve the development of one or more system models and prototypes. These help you understand the system to be specified.
3. *Requirements specification* - Requirements specification is the activity of translating the information gathered during the analysis activity into a document that defines a set of requirements. Two types of requirements may be included in this document. User requirements are abstract statements of the system requirements for the customer and end-user of the system; system requirements are a more detailed description of the functionality to be provided.
4. *Requirements validation* - This activity checks the requirements for realism, consistency, and completeness. During this process, errors in the requirements document are inevitably discovered. It must then be modified to correct these problems.
