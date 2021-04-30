# Second Demonstration

  * Date: May 7th
  * Examiners: Philippe Collet, Guilhem Molines, Anne-Marie Pinna, Nikita Rousseau

## Planning

  * Constraints: 
    * 15 minutes for the team, around 15 minutes for the jury (for questions)
    * Remote

  * Planning:
  
| Timeslot      | Jury 1 + 2    |
|---------------|---------------|
| 08:00 - 08:30 | Team  I       | 

| Timeslot      | Jury 1  | 
|---------------|---------| 
| 08:45 - 09:15 | Team  O |
| 09:15 - 09:45 | Team  M |
| 09:45 - 10:15 | Team  L |
| 10:15 - 10:45 | Team  J | 
| 10:45 - 11:00 | Break   | 
| 11:00 - 11:30 | Team  D |
| 11:30 - 12:00 | Team  B |
| 12:00 - 12:30 | Team  C |
| 12:30 - 13:00 | Team  A |

| Timeslot      | Jury 2  | 
|---------------|---------| 
| 08:45 - 09:15 | Team  Q |
| 09:15 - 09:45 | Team  P |
| 09:45 - 10:15 | Team  N |
| 10:15 - 10:45 | Team  K | 
| 10:45 - 11:00 | Break   | 
| 11:00 - 11:30 | Team  H |
| 11:30 - 12:00 | Team  G |
| 12:00 - 12:30 | Team  F |
| 12:30 - 13:00 | Team  E |


## Expectations

You have to demonstrate a single product, covering both ISA & DevOps course contents. This single demo will be evaluated according to these two dimensions, leading to two different marks. *However*, the two courses expect the project to respect the call for bids and implement features related to this project.

Think about demonstrating error cases (e.g., third party service unavailable, network lost, broken test, corrupted JAR, ...) instead of staying in a perfect world. 

  * For *ISA*, the keypoint is to demonstrate a comprehensive architecture, going from the persistence layer to the exposition one (_i.e._, web services, CLI or other interface). You must be able to defend the strengths of your architecture, as well as discuss its limitations and evolution capabilities. You can follow the previous points put on the slack:
     * presentation of evolution of the architecture, its decomposition into components (and especially *why they are decomposed in this way*), the scenario of the demonstration
     * explanation of the impact of the integration of persistence
     * evolution of stateless/ful components
     * Where and why did you integrate interceptors (or where/why it could have be done, if you did not have time to do so)
     * Where and why did you integrate communication by messages (or where/why it could have be done, if you did not have time to do so)
     * Live demo is *mandatory*
     * While showing BDD tests to demonstrate functionalities, relying only on them is not a good idea to demonstrate the CLI.
    
  * For *DevOps*, you demonstrated during the first demo that you master a Continuous Integration system. For demo 2, we expect to see a Continuous Delivery system. By that, we mean to see a fully instrumented pipeline, that not only compiles the code, but also proves it correct through various levels of testing and generates the product deliverables. Special attention will be paid to integration tests (end2end testing from ws to backend and external systems is priority #1). We expect the core product deliverable to be in the form of (at least two) docker images, and launchable through a simple command line [we do not place the docker requirement on the clients and the external servers, but launching them should be trivial as well]. Docker Compose is mandatory. There is no requirement on any scaling technology such as Swarm or Kubernetes. Be ready to answer questions on your testing and branching strategies.

You must also clearly identify who did what (for both topics) in the project development.
