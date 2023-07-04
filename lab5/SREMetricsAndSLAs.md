# List and explain the key metrics used in SRE.

1. Service-Level Objective (SLO) - target service level
This indicator can be both a low vice (for example, users will not notice a difference or notice, but this will not affect their satisfaction with the service) and high, when users flood the chats that the service is unavailable or any action on the service is several times slower than usual
2. Service Level Indicator (SLI) - it could be response time, error percentage, throughput, response correctness, anything depending on the product.
3. Service Level Agreement (SLA) - This agreement describes the health of the entire service and penalties for exceeding downtime or other violations.
Exmpl: SLA: service is available 98% of the time throughout the 3 month; 80 support ticket gaps will be closed within three hours in two months; 60% of incoming responses within 10 minutes each time.
4. MTBF (Mean Time Between Failures) - the average time between failures
5. MTTR (Mean Time To Recovery) - the average recovery time (how long it took from the appearance of an error to a rollback to normal operation).
The SRE engineer influences him through automation. For example, SLO has a 98% quarterly uptime, which means the team has 86 minutes of downtime for 3 months.
In this case, the recovery time cannot be more than 86 minutes, otherwise the entire “budget” for the quarter will be exhausted in one incident, the SLO will be violated.
# Share the SLAs or reliability metrics you found for the two companies, along with any notable observations or insights.
1. Google Workspace
https://workspace.google.com/terms/sla.html
2. Yandex translate
https://translate.yandex.com/developers/offer/sla
3. Microsoft Azure SLA
https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services?lang=1
# Discuss the importance of these metrics and how they contribute to the overall reliability and performance of software systems.
SRE works wherever you need to roll out updates, change infrastructure, grow and scale. 
SRE engineers help to predict and identify possible growth issues. Therefore, they are needed even in those companies where the main activity is not software development.
At the same time, it is not necessary to hire an individual person for the SRE role, you can make the role transitional, or you can grow a person within the team. The last option is suitable for startups.
When a company plans to grow tenfold, then a person is needed who is responsible for ensuring that nothing breaks with a given growth.

You can implement SRE principles from a small point: define SLO, SLI, SLA and set up monitoring. If the company is not engaged in software, then these will be
internal SLAs and internal SLOs. Discussion of these agreements leads to interesting discoveries. It often turns out that a company spends much more time and effort on the infrastructure or organization of ideal processes than it should.

In addition, it is good for any company to accept that mistakes are normal and start working on them. Determine the Error budget, try to spend it on development, and analyze the problems that arise and, based on the results of the analysis, implement automation.

# References:
1. https://cloud.google.com/blog/products/devops-sre/sre-fundamentals-slis-slas-and-slos
2. https://cloud.google.com/blog/products/devops-sre/sre-fundamentals-sli-vs-slo-vs-sla
3. https://cloud.google.com/blog/products/devops-sre/availability-part-deux-cre-life-lessons