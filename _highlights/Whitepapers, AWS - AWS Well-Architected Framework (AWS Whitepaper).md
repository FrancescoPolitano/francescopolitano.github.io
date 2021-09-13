# AWS Well-Architected Framework (AWS Whitepaper)
by Whitepapers, AWS

46 highlights

---

* set of foundational questions that allow you to understand if a specific architecture aligns well with cloud best practices.

<p style="text-align: right;"><sup>highlight @ page 5, loc. 91-92</sup></p>

* To help you apply best practices, we have created AWS Well-Architected Labs, which provides you with a repository of code and documentation to give you hands-on experience implementing best practices.

<p style="text-align: right;"><sup>highlight @ page 6, loc. 112-115</sup></p>

* set of best practices for customers and partners to evaluate architectures, and provides a set of questions you can use to evaluate how well an architecture is aligned to AWS best practices.

<p style="text-align: right;"><sup>highlight @ page 7, loc. 127-129</sup></p>

* The AWS Well-Architected Framework is based on ﬁve pillars — operational excellence, security, reliability, performance efficiency, and cost optimization.

<p style="text-align: right;"><sup>highlight @ page 7, loc. 129-131</sup></p>

* support development and run workloads effectively, gain insight into their operations, and to continuously improve supporting processes and procedures to deliver business value.

<p style="text-align: right;"><sup>highlight @ page 7, loc. 135-136</sup></p>

* take advantage of cloud technologies to improve your security.

<p style="text-align: right;"><sup>highlight @ page 8, loc. 137-138</sup></p>

* the ability of a workload to perform its intended function correctly and consistently when it’s expected to.

<p style="text-align: right;"><sup>highlight @ page 8, loc. 139-140</sup></p>

* The ability to use computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.

<p style="text-align: right;"><sup>highlight @ page 8, loc. 142-143</sup></p>

* A component is the code, configuration, and AWS Resources that together deliver against a requirement.

<p style="text-align: right;"><sup>highlight @ page 8, loc. 147-149</sup></p>

* The term workload is used to identify a set of components that together deliver business value.

<p style="text-align: right;"><sup>highlight @ page 8, loc. 152-153</sup></p>

* We think about architecture as being how components work together in a workload.

<p style="text-align: right;"><sup>highlight @ page 9, loc. 155-156</sup></p>

* Milestones mark key changes in your architecture as it evolves throughout the product lifecycle

<p style="text-align: right;"><sup>highlight @ page 9, loc. 159-160</sup></p>

* Within an organization the technology portfolio is the collection of workloads that are required for the business to operate.

<p style="text-align: right;"><sup>highlight @ page 9, loc. 162-165</sup></p>

* Security and operational excellence are generally not traded-oﬀ against the other pillars.

<p style="text-align: right;"><sup>highlight @ page 9, loc. 168-170</sup></p>

* At AWS, we prefer to distribute capabilities into teams rather than having a centralized team with that capability.

<p style="text-align: right;"><sup>highlight @ page 9, loc. 179-180</sup></p>

* The Well-Architected Framework identifies a set of general design principles to facilitate good design in the cloud:

<p style="text-align: right;"><sup>highlight @ page 13, loc. 224-226</sup></p>

* Stop guessing your capacity needs:

<p style="text-align: right;"><sup>highlight @ page 13, loc. 226-227</sup></p>

* Test systems at production scale: In the cloud, you can create a production-scale test environment on demand, complete your testing, and then decommission the resources.

<p style="text-align: right;"><sup>highlight @ page 13, loc. 232-233</sup></p>

* Drive architectures using data: In the cloud, you can collect data on how your architectural choices affect the behavior of your workload. This lets you make factbased decisions on how to improve your workload.

<p style="text-align: right;"><sup>highlight @ page 13, loc. 248-250</sup></p>

* Improve through game days: Test how your architecture and processes perform by regularly scheduling game days to simulate events in production.

<p style="text-align: right;"><sup>highlight @ page 14, loc. 253-255</sup></p>

* There are ﬁve design principles for operational excellence in the cloud:

<p style="text-align: right;"><sup>highlight @ page 15, loc. 273-274</sup></p>

* Perform operations as code:

<p style="text-align: right;"><sup>highlight @ page 15, loc. 274-275</sup></p>

* Make frequent, small, reversible changes: Design workloads to allow components to be updated regularly.

<p style="text-align: right;"><sup>highlight @ page 16, loc. 281-282</sup></p>

* Refine operations procedures frequently

<p style="text-align: right;"><sup>highlight @ page 16, loc. 284-285</sup></p>

* Anticipate failure:

<p style="text-align: right;"><sup>highlight @ page 16, loc. 289-289</sup></p>

* Learn from all operational failures:

<p style="text-align: right;"><sup>highlight @ page 16, loc. 294-295</sup></p>

* Organization Your teams need to have a shared understanding of your entire workload, their role in it, and shared business goals to set the priorities that will enable business success. Well-defined priorities will maximize

<p style="text-align: right;"><sup>highlight @ page 17, loc. 314-316</sup></p>

* Ensure that there are identified owners for each application, workload, platform, and infrastructure component, and that each process and procedure has an identified owner responsible for its definition, and owners responsible for their performance.

<p style="text-align: right;"><sup>highlight @ page 18, loc. 334-337</sup></p>

* Teams must grow their skill sets to adopt new technologies, and to support changes in demand and responsibilities. Support and encourage this by providing dedicated structure time for learning.

<p style="text-align: right;"><sup>highlight @ page 20, loc. 348-350</sup></p>

* AWS Trusted Advisor is a tool that provides access to a core set of checks that recommend optimizations that may help shape your priorities

<p style="text-align: right;"><sup>highlight @ page 20, loc. 364-365</sup></p>

* You should use tools or services that enable you to centrally govern your environments across accounts, such as AWS Organizations, to help manage your operating models. Services like AWS Control Tower expand this management capability by enabling you to define blueprints (supporting your operating models) for the setup of accounts, apply ongoing governance using AWS Organizations

<p style="text-align: right;"><sup>highlight @ page 21, loc. 374-376</sup></p>

* Adding Managed Services to your operating model can save you time and resources, and lets you keep your internal teams lean and focused on strategic outcomes that will differentiate your business, rather than

<p style="text-align: right;"><sup>highlight @ page 22, loc. 379-381</sup></p>

* Adding Managed Services to your operating model can save you time and resources, and lets you keep your internal teams lean and focused on strategic outcomes that will differentiate your business, rather than developing new skills and capabilities.

<p style="text-align: right;"><sup>highlight @ page 22, loc. 379-382</sup></p>

* Have shared goals in order to set priorities for resources. This will maximize the benefits of your efforts.

<p style="text-align: right;"><sup>highlight @ page 22, loc. 386-387</sup></p>

* achieving business outcomes. Teams need to understand their roles in the success of other teams, the role of other teams in their success, and have shared goals.

<p style="text-align: right;"><sup>highlight @ page 22, loc. 389-390</sup></p>

* Provide support for your team members so that they can be more effective in taking action and supporting your business outcome.

<p style="text-align: right;"><sup>highlight @ page 22, loc. 393-395</sup></p>

* Organizational culture has a direct impact on team member job satisfaction and retention.

<p style="text-align: right;"><sup>highlight @ page 23, loc. 399-400</sup></p>

* Adopt approaches that improve the ﬂow of changes into production and that enable refactoring, fast feedback on quality, and bug fixing.

<p style="text-align: right;"><sup>highlight @ page 23, loc. 411-412</sup></p>

* Evaluate the operational readiness of your workload, processes, procedures, and personnel to understand the operational risks related to your workload.

<p style="text-align: right;"><sup>highlight @ page 24, loc. 420-421</sup></p>

* Design your workload so that it provides the information necessary across all components (for example, metrics, logs, and traces) for you to understand its internal state. This enables you to provide effective responses when appropriate.

<p style="text-align: right;"><sup>highlight @ page 25, loc. 434-436</sup></p>

* Adopt approaches that provide fast feedback on quality and enable rapid recovery from changes that do not have desired outcomes

<p style="text-align: right;"><sup>highlight @ page 25, loc. 442-443</sup></p>

* Evaluate the operational readiness of your workload, processes and procedures, and personnel to understand the operational risks related to your workload.

<p style="text-align: right;"><sup>highlight @ page 25, loc. 446-448</sup></p>

* Invest in implementing operations activities as code to maximize the productivity of operations

<p style="text-align: right;"><sup>highlight @ page 25, loc. 448-448</sup></p>

* Use “pre-mortems” to anticipate failure and create procedures where appropriate.

<p style="text-align: right;"><sup>highlight @ page 25, loc. 449-449</sup></p>

* Apply metadata using Resource Tags and AWS Resource Groups following a consistent tagging strategy to enable identification of your resources.

<p style="text-align: right;"><sup>highlight @ page 25, loc. 449-450</sup></p>

* Adopt deployment practices that take advantage of the elasticity of the cloud to facilitate development activities, and pre-deployment of systems for faster implementations.

<p style="text-align: right;"><sup>highlight @ page 25, loc. 451-452</sup></p>

