
---

# Stakeholders

In the original kata documentation, there are different stakeholders/users mentioned.

- Civilian
- Police officer
- Charities (non-profit organization)
- Retail Organizations (for-profit organization)

## Stakeholder Concerns

The following are the concerns from described stakeholders of the system.

These will be informative in deciding the [architectural characteristics](ArchitectureAnalysis.md) and informing decisions on the architecture of the Hey Blue App.

| Stakeholder               | Concerns                                                                                         | Initial Thoughts on Characteristics/Generics     |
| ------------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------------------ |
| SH-1: Civilian     | - Ease of use for everyone<br/>- Social media integration<br/>- Connectivity with officers and retails<br/>- Location tracked in order to notify of nearby police or retails<br/>- Protect user data , what to store and what is transient        | Accessibility, Usability, Availability, Reliability, Interoperability, Archivability, Scalability |
| SH-2: Police Officer      | - Ease of use<br/>- Data protection<br/>- Can control visibility of their geolocation                          | Data Integrity, Abstraction, Fault-tolerance |
| SH-3: Non-profit Organization             | - Analytics/reporting<br/>- Ability to create storefront                                         | Workflow |
| SH-4: For-profit Organization | - Ability to create storefront<br/>- Affiliate support <br/>-Process payments for goods                                          | Workflow, Abstraction, Interoperability |

