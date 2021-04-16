# Introduction to Software Architecture (2020-21)

## Teaching Staff

  * [Philippe Collet](collet@i3s.unice.fr), Université Côte d'Azur, CNRS, I3S (co-head, ISA)
  * [Anne-Marie Pinna-Déry](pinna@unice.fr), Université Côte d'Azur, CNRS, I3S
  * Nassim Bounouas (AL 2019), SQUAD/Orange, Université Côte d'Azur (ISA)
  * Laura Lopez (AL 2020), Greencom Networks, Université Côte d'Azur (ISA)
  * Nathan Strobbe (AL 2020), TriPica, Université Côte d'Azur (ISA)


## Lecture Material

  - Lecture #1: Kick-off / N-tiers Architecture / UML support / JavaEE and EJB Basics: [videos (Panopto) are on LMS](https://lms.univ-cotedazur.fr/course/view.php?id=4332&section=1)
    - 1.1 [Kick-off](https://github.com/collet/isa-devops/blob/master/ISA/1.1_isa_kickoff.pdf)
    - 1.2 [N-tiers architecture / Layered architecture / UML support](https://github.com/collet/isa-devops/blob/master/ISA/1.2_isa_Archi_N_Tiers.pdf)
    - 1.3 [JavaEE / EJB Basics](https://github.com/collet/isa-devops/blob/master/ISA/1.3_isa_javaEE-ejb-partie1.pdf)  [Dependency injection](https://github.com/collet/isa-devops/blob/master/ISA/1.3_isa_javaEE-ejb-partie2.pdf)
  - Lecture #2: ORM 101 / Session beans 101: [videos (Panopto) are on LMS](https://lms.univ-cotedazur.fr/course/view.php?id=4332&section=1)
    - 2.1 [ORM 101](https://github.com/collet/isa-devops/blob/master/ISA/2_1_isa_orm.pdf)
    - 2.2 [Session beans 101](https://github.com/collet/isa-devops/blob/master/ISA/2_2_isa_sessionBeans.pdf)
  - Lecture #3: C/S and Architectural viewpoints
  	 - 3.1 [Remoting and C/S](https://github.com/collet/isa-devops/blob/master/ISA/3_1_ISARemote2021.pdf)
  	 - 3.2 [Architectural viewpoints](https://github.com/collet/isa-devops/blob/master/ISA/3_2_ISAViewpoints2021.pdf) 
  - Lecture #4: Stateful and stateless session beans
    - [State Wars](https://github.com/collet/isa-devops/blob/master/ISA/4_stateWars.pdf)
  - Lecture #5: Persistence
    - 5.1 [Persistence - Entity and Id](https://github.com/collet/isa-devops/blob/master/ISA/5_persistence-part1.pdf)
    - 5.2 [Persistence - Relation and Inheritance](https://github.com/collet/isa-devops/blob/master/ISA/5_persistence-part2.pdf)
    - 5.3 [Persistence - Entity Manager](https://github.com/collet/isa-devops/blob/master/ISA/5_persistence-part3.pdf)
    - 5.4 [Persistence - Advanced tricks](https://github.com/collet/isa-devops/blob/master/ISA/5_persistence-part4.pdf)
  - Lecture #6: Interceptors and MOM
    - [Interceptors and MOM](https://github.com/collet/isa-devops/blob/master/ISA/6_j2e_plus_plus.pdf) 

### Examples of _good_ architecture reports (FR):

  - 2017: Disloyalty card. [Report #1](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2017_1.pdf) [Report #2](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2017_2.pdf)
  - 2019: Graduation ceremony. [Report #1](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2019_1.pdf) [Report #2](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2019_2.pdf)
  - 2020: Drone delivery. [Report #1](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2020_1.pdf) [Report #2](https://github.com/collet/isa-devops/blob/master/ISA/reports_examples/2020_2.pdf)
  
## Assignment #1

First Assignment requires you to compile and package the code base of The Cookie Factory. The code base is available [in this repository (develop branch)](https://github.com/collet/4A_ISA_TheCookieFactory).

## Assignment #2

Build an architecture report for the case study.

## Deliverables

### Architecture Report (first report)

You must deliver a PDF file *in the slack channel of your team*, named `architecture-team-X.pdf` where X is your team letter. There is no page limit but _concision_ is an evaluation criterion (and your report should be ~10 pages long): *Sunday 14th, February, 8:00pm*

It must contain the following architecture description:

  - Use cases diagrams;
  - Business objects definition as class diagram;
  - Interfaces pseudo-code definition (_e.g._, Java like);
  - Components described by a component diagram;

Each artefact must be justified with respect to its relevance in your architecture.

Non-exhaustive list of common pitfalls to avoid in your work:

  - spending (way) too much time on use cases definition and description;
  - defining interfaces and components that do not support than _business_;
  - Weird responsibilities for components (_e.g._, god component, disconnected assemblies, dangling element)
  - Lack of proper description/justification for the interfaces
  - Interfaces that relies on _ids_ and primitive objects (_e.g._, String, Integers) instead of business objects.


### Final Project Delivery (deadline: May 9th, 6:00pm)

  - you need to deliver according to the instructions of the DevOps part +
  - You must deliver a PDF file at the root of your main repository on Github, named `finalreport-teamX.pdf` where X is your team letter. There is no page limit, but concision is an evaluation criteria (and your report should be ~10 pages long). You must be able to defend the strengths of your architecture, as well as discuss its limitations and evolution capabilities. You can base your defense on the evolution of          
      - the component diagram; 
      - interfaces;
      - class diagram;
      - the implementation and/or design choice of persistence, interceptors, the three types of components (Stateful, stateless, oriented messages)
  - Each artefact (component, interface, class for persisted entity) must be justified with respect to its relevance in your architecture.
  - the deliverable for both ISA and DevOps will be extracting using a specific script. Make sure your git repository tag is correct (see DevOps part as well).
  
  
  
  
