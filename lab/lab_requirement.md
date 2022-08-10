# OPI lab requirements

| DESCRIPTION                                                                                                                            | LABELS             | STAKEHOLDER                 | PRIORITY (1=most important) | COMMENT                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | --------------------------- | ------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| Can ssh to server from various OPI member vpns                                                                                         | ACCESS             | COMMON                      | 1                              |                                                                                                              |
| Raritan in place for all servers                                                                                                       | ACCESS             | SYS\_ADMIN                  |                                | To enable remote access to servers in case main network is down.                                             |
| Secondary remote management system enabled to supplement Raritan.  System must support firmware updates.                               | ACCESS             | SYS\_ADMIN                  |                                | For example, Dell's iDRAC (Dell Remote Access Controller)                                                    |
| Remote access to power cyclers                                                                                                         | ACCESS             | SYS\_ADMIN, DEV, VALIDATION |                                |                                                                                                              |
| Wiki showing servers, assigned owners, raritan info, ssh access info                                                                   | ACCESS, DOC        | COMMON                      |                                |                                                                                                              |
| All critical servers backed up                                                                                                         | BACKUP             | COMMON                      |                                |                                                                                                              |
| Restore of critical servers must be done within a couple of hours                                                                      | BACKUP             | COMMON                      |                                |                                                                                                              |
| Team in place trained to do backup/restore                                                                                             | BACKUP             | COMMON                      |                                |                                                                                                              |
| Sufficient capacity so wait queue is zero to accommodate all CI workloads                                                              | CAPACITY, CICD     | DEV, VALIDATION             |                                | processing resources need to be proportional to rate of GitHub PR arrivals x average time to do builds+tests |
| Sufficient excess capacity so as new users request lab capacity they can be reasonably accomodated without waiting                     | CAPACITY, CICD     | DEV, VALIDATION             |                                |                                                                                                              |
| Complies with all laws in jurisdiction where data center is hosted                                                                     | COMPLIANCE         | COMMON                      |                                | E.g., need to seismic the racks if located in California                                                     |
| Complies with all data privacy laws                                                                                                    | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with HIPAA (health information)                                                                                               | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with National Institute of Technology (NIST) and Uptime Institute's certification tiers                                       | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with quality standareds, like ISO                                                                                             | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with security standards, like SOC                                                                                             | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with environmental management standards                                                                                       | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Complies with energy eifficent data center designs                                                                                     | COMPLIANCE         | COMMON                      |                                | Not an expert on this.  Came up from google search.                                                          |
| Documentation in place for browsing, requesting, and releasing lab resources                                                           | DOC                | DEV, VALIDATION             |                                | E.g., how to request for new physical servers with power cycler                                              |
| Documentation in place for lab resources and interconnections                                                                          | DOC                | DEV, VALIDATION             |                                | For example <https://opendcim.org/screenshots>.html                                                            |
| Storage area/bins in place to cache supply of lab equipement, such as cables, optical transceivers, hard drives, RAM, usb sticks, etc. | FACILITIES         | TECH                        |                                |                                                                                                              |
| HVAC in place with sufficient capacity to dissipate heat                                                                               | FACILITIES         | COMMON                      |                                | 3 ton HVAC not sufficient for 4 racks.  Need at least 5 tuns for 4 racks.                                    |
| Electrical power in place with sufficient capacity to service all lab equipment                                                        | FACILITIES         | COMMON                      |                                |                                                                                                              |
| Sufficient power outlets so all equipment needing outlet is accounting for, inclusive of failover power supplies                       | FACILITIES, BACKUP | COMMON                      |                                |                                                                                                              |
| Poster identifying meaning of cable color codes                                                                                        | FACILITIES, DOC    | TECH                        |                                |                                                                                                              |
| Redundant HVAC in place in case primary HVAC dies                                                                                      | FACILITIES, BACKUP | COMMON                      |                                |                                                                                                              |
| From servers, can access CI controller (e.g. Jenkins)                                                                                  | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| From servers, can access K8s cluster                                                                                                   | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| From servers, can access Artifactory                                                                                                   | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| From servers, can access JIRA                                                                                                          | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| From servers, can access open source repos                                                                                             | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| From servers, can access various databases                                                                                             | NETWORK            | DEV, VALIDATION             |                                |                                                                                                              |
| End users given 2 week notice for major lab works                                                                                      | PROCESS            | COMMON                      |                                |                                                                                                              |
| End users given 1 week notice for regular lab maintenance works                                                                        | PROCESS            | COMMON                      |                                |                                                                                                              |
| End users notified as soon as it is known immediate emergency lab work need to be done                                                 | PROCESS            | COMMON                      |                                |                                                                                                              |
| Firedrills scheduled to refresh operational knowledge to deal with emergency events                                                    | PROCESS            | COMMON                      |                                |                                                                                                              |
| Lab inventory management system in place                                                                                               | PROCESS            | COMMON                      |                                |                                                                                                              |
| Lab tech updates inventory as needed                                                                                                   | PROCESS            | COMMON                      |                                |                                                                                                              |
| Lab manager assigned                                                                                                                   | PROCESS            | COMMON                      |                                |                                                                                                              |
| Process in place to forecast equipment needs                                                                                           | PROCESS            | COMMON                      |                                |                                                                                                              |
| Questionnaire in place to be handed out to lab users to help with equipment forecast                                                   | PROCESS            | MANAGEMENT                  |                                |                                                                                                              |
| Lab requirements reviewed by OPI TSC                                                                                                   | PROCESS            | COMMON                      |                                |                                                                                                              |
| Sufficient budget in place to fund initial capital costs                                                                               | PROCESS            | MANAGEMENT                  |                                |                                                                                                              |
| Sufficient budget in place to fund ongoing operations                                                                                  | PROCESS            | MANAGEMENT                  |                                |                                                                                                              |
| Complies with operational security policies                                                                                            | SECURITY           | COMMON                      | 1                              | e.g. card key access                                                                                         |
| Authentication done through centralized system, such as Kerberos, as much as possible                                                  | SECURITY           | COMMON                      |                                |                                                                                                              |
| Authorization done through centralized system such as LDAP, as much as possible                                                        | SECURITY           | COMMON                      |                                |                                                                                                              |
| Ticketing system in place to request lab services                                                                                      | PROCESS            | COMMON                      |                                |                                                                                                              |
| ssh access at 99.99% availability                                                                                                      | SLA                | COMMON                      |                                |                                                                                                              |
| Lab tech accessible 24/7                                                                                                               | SLA                | COMMON                      |                                | This implies covers all timezones.                                                                           |
|                                                                                                                                        |                    |                             |                                |                                                                                                              |