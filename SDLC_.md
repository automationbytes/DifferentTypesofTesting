# Software Development Life Cycle (SDLC)

## Stages of SDLC:

1. **Requirements Gathering:** Collect and analyze the requirements from stakeholders.
2. **Design:** Create architecture and design specifications.
3. **Implementation (Coding):** Write and integrate the code for the project.
4. **Testing:** Test the software to identify defects and ensure quality.
5. **Deployment:** Deploy the software to the production environment.
6. **Maintenance:** Provide ongoing support, fix bugs, and make updates.

## SDLC Diagram:

```mermaid
graph TD;
    Requirements --> Design;
    Design --> Implementation;
    Implementation --> Testing;
    Testing --> Deployment;
    Deployment --> Maintenance;


## Simplified SDLC Process Document

| Phase                    | Input                                                  | What Happens Here                                                        | Who's In Charge               | Outcome/Deliverables         |
|--------------------------|--------------------------------------------------------|--------------------------------------------------------------------------|-------------------------------|------------------------------|
| **Requirement**             | Business Requirements, Stakeholder Input               | - Decide what the project should do                                      | Project Manager               | Project Plan                 |
|                          |                                                        | - Figure out who will be involved and what is needed                     | Business Analyst              | Budget and Timeline          |
|                          |                                                        | - Estimate costs and set the budget                                      | Finance Team                  |                              |
|                          |                                                        | - Create a timeline for the project                                      | Project Manager               |                              |
| **Feasibility Study**    | Business Requirements, Project Plan                    | - Check if the project is technically possible                           | System Architect              | Feasibility Report           |
|                          |                                                        | - Determine if it's economically and legally feasible                    | Legal and Financial Teams     |                              |
|                          |                                                        | - Assess if it can be operationally managed                              | Operations Team               |                              |
| **System Design**        | Approved Feasibility Study, System Requirements        | - Plan how the system will look and work                                 | System Architect              | Design Documents             |
|                          |                                                        | - Design the database                                                    | Database Administrator        |                              |
|                          |                                                        | - Create prototypes                                                      | UI/UX Designers               | Prototypes                   |
|                          |                                                        | - Review and approve the designs                                         | Design Review Team            |                              |
| **Implementation**       | Design Documents, Prototypes                           | - Write the code for the system                                          | Development Team              | Source Code                  |
|                          |                                                        | - Manage versions and document the code                                  | Configuration Manager         |                              |
|                          |                                                        | - Review and test the code                                               | Development and QA Teams      |                              |
|                          |                                                        | - Integrate different parts of the code                                  | Development Team              |                              |
| **Integration & Testing**| Source Code, Test Plan, Test Cases                     | - Combine all parts of the system                                        | Integration Team              | Integrated System            |
|                          |                                                        | - Test the system to make sure it works                                  | QA Team                       | Test Results                 |
|                          |                                                        | - Test the system’s performance                                          | Performance Testing Team      |                              |
|                          |                                                        | - Test the system’s security                                             | Security Testing Team         |                              |
|                          |                                                        | - Fix bugs and retest                                                    | Development Team              |                              |
| **Deployment**           | Integrated System, Deployment Plan                     | - Plan and execute the deployment                                        | Deployment Team               | Deployed System              |
|                          |                                                        | - Train users on the new system                                          | Training Team                 |                              |
|                          |                                                        | - Monitor the system after deployment                                    | IT Operations Team            |                              |
| **Maintenance**          | Deployed System, User Feedback                         | - Provide ongoing support and maintenance                                | Maintenance Team              | System Updates               |
|                          |                                                        | - Monitor the system’s performance                                       | Support Team                  |                              |
|                          |                                                        | - Fix bugs and make improvements                                         | Development Team              |                              |
|                          |                                                        | - Provide regular updates and patches                                    | Maintenance Team              |                              |
