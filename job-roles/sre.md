# Site Reliability Engineer

Site Reliability Engineers (SREs) are responsible for keeping all user-facing services and other MayaData production systems running smoothly. SREs are a blend of pragmatic operators and software craftspeople that apply sound engineering principles, operational discipline, and mature automation to our environments and the MayaData codebase. 

Our vision is to enable a new era of workload based data management by turning Kubernetes itself into a data plane.  This use of Kubernetes as the data plane boosts the productivity and control of software development groups while decreasing cloud and vendor lock-in.

We focus on the jobs that our users need to get done in order to trust Kubernetes as their data layer.  Specifically, we focus upon:
- Ease of deployment and operations of stateful workloads on Kubernetes
- Simplicity of data protection including replicas, back-ups and data migration
- Automatic and seamless protection from lock-in, via background rebalancing or on demand data migration

MayaData has several user facing sites that include many websites, documentation portals, build/CI platforms and a biggest OpenEBS storage powered SaaS Platform - called OpenEBS Director. In fact, OpenEBS Director is one of the largest SaaS sites providing Storage observability to serveral Kubernetes clusters across the world. OpenEBS Director is also delivered as a software product, to be installed in user's premises. 

All of our workloads are powered with Kubernetes and OpenEBS Storage. The experience of our team feeds back into other engineering groups within the company, as well as to MayaData customers running self-managed installations of OpenEBS and OpenEBS Director.

**As an SRE you will:**
- Be on a PagerDuty/Slack rotation to respond to MayaData availability incidents and provide support for service engineers with customer incidents.
- Use your on-call shift to prevent incidents from ever happening.
- Run our infrastructure with Ansilbe, Terraform, GitOps and Kubernetes.
- Make monitoring and alerting alert on symptoms and not on outages.
- Document every action so your findings turn into repeatable actions–and then into automation.
- Use the MayaData products to run Director as a first resort and improve the product as much as possible
- Improve the deployment process to make it as boring as possible.
- Design, build and maintain core infrastructure pieces that allow MayaData scaling to support hundred of thousands of concurrent users.
- Debug production issues across services and levels of the stack.
- Plan the growth of MayaData's infrastructure.

**You may be a fit for this role if you:**
- Think about systems - edge cases, failure modes, behaviors, specific implementations.
- Know your way around Kubernetes, Grafana, Prometheus, MySQL, Cassandra, Linux and the Unix Shell.
- Know what is the use of config management systems like GitHub, GitLab, Ansible
- Have strong programming skills - Python and/or Go
- Have an urge to collaborate and communicate asynchronously.
- Have an urge to document all the things so you don't need to learn the same thing twice.
- Have an enthusiastic, go-for-it attitude. When you see something broken, you can't help but fix it.
- Have an urge for delivering quickly and iterating fast.
- Share our values, and work in accordance with those values.
- Have experience with GKE, Nginx, HAProxy, Docker, Kubernetes, Terraform, or similar technologies
- Ability to use MayaData products like OpenEBS, Litmus, Director
- You love sharing your learnings with other folks within and outside the company through Meetups, Conference talks and so forth. 

**Projects you could work on:**
- Coding infrastructure automation with Terraform, Ansible, Python and other SaaS products
- Improving our Prometheus Monitoring or building new Metrics
- Helping release managers deploy and fix new versions of Director and OpenEBS.
- Helping customers manage their solutions/installations of OpenEBS and OpenEBS Director. 
- Plan, prepare for, and execute the migration of Stateful Workloads running on OpenEBS and Director on Kubernetes - handling the upgrades and auto-scaling of Kubernetes Clusters, Geo-distribution of the applications.
- Plan and automate setting up of Stateful Workloads on Kubernetes on different platforms from virtual machines to different cloud providers like - GKE, AKS, AWS, OpenShift.
- Develop a relationship with a product group, define their SLAs, share Mayadata production sites data on those SLAs and improve their reliability

## Leveling of Site Reliability Engineering

**Technical:** 
- Use automation to efficiently manage our fleet of servers
- Implement "Infrastructure as Code" using Terraform, Flux, Helm and GitLab/Jenkins/Travis CI/CD, for automation
- Kubernetes and containerizing our system
- Product knowledge of OpenEBS, Director, Litmus and the eco-system products deployed on Director. 
- Monitoring and Metrics in Prometheus, Grafana and integrations with Slack/PagerDuty
- Logging infrastructure
- Running Stateful Workloads at scale using OpenEBS, along with Infrastructure and Storage Management
- Disaster Recovery and High Availability strategy
- Contributing to code in MayaData

**Execution:**
- Team organization and planning
- Issue, Epic, OKR leadership and completion

**Collaboration and Communication:**
- Creating blog posts
- Completing Root Cause Analysis (RCA) investigations
- Contributions to handbook, runbooks, general documentation
- Leading and contributing to designs for issues, epics, okrs
- Improving team practices in handoffs of work and incidents

**Influence and Maturity**
- Involvement in the hiring process - reviewing questionnaires, involved in interviews, qualifying candidates
- Knowledge sharing, mentoring
- Accountability, Self awareness, handling conflict in the team and receiving feedback
- Maintaining good relationships with other engineering teams in MayaData that help improve the product


## Levels for Site Reliability Engineer

### Junior Site Reliability Engineer

**Technical:**
- Updates MayaData Director and OpenEBS default values so there is no need for configuration by customers.
- General knowledge of the 2 of the areas of technical expertise

**Execution:**
- Provides emergency response either by being on-call or by reacting to symptoms according to monitoring and escalation when needed
- Delivers production solutions that scale, identifies automation points, and proposes ideas on how to improve efficiency.
- Improves monitoring and alerting fighting alert spam.

**Collaboration and Communication:**
- Improves documentation all around, either in application documentation, or in runbooks, explaining the why, not stopping with the what.

**Influence and Maturity**
- Shares the learnings publicly, either by creating issues that provide context for anyone to understand it or by writing blog posts.

### Site Reliability Engineer

**Technical:**
- General knowledge of the 4 of the areas of technical expertise with deep knowledge in 1 area

**Execution:**
- Provides emergency response either by being on-call or by reacting to symptoms according to monitoring and escalation when needed
- Proposes ideas and solutions within the infrastructure team to reduce the workload by automation.
- Plan, design and execute solutions within the infrastructure team to reach specific goals agreed within the team.
- Plan and execute configuration change operations both at the application and infrastructure level.
- Actively looks for opportunities to improve the availability and performance of the system by applying the learning from monitoring and observation

**Collaboration and Communication:**
- Improves documentation all around, either in application documentation, or in runbooks, explaining the why, not stopping with the what.

**Influence and Maturity:**
- Shares the learnings publicly, either by creating issues that provide context for anyone to understand it or by writing blog posts.
- Contributes to the hiring process in review questionnaires or being part of the interview team to qualify SRE candidates

### Senior Site Reliability Engineer

**Technical:** 
- Deep knowledge in 2 areas of expertise and general knowledge of all areas of expertise. Capable of mentoring Junior in all areas and other SRE in their area of deep knowledge.
- Contributes small improvements to the MayaData codebase to resolve issues

**Execution:**
- Identifies significant projects that result in substantial cost savings or revenue
- Identifies changes for the product architecture from the reliability, performance and availability perspective with a data driven approach.
- Proactively work on the efficiency and capacity planning to set clear requirements and reduce the system resources usage to make OpenEBS and Director cheaper to run for all our customers.
- Identify parts of the system that do not scale, provides immediate palliative measures and drives long term resolution of these incidents.
- Identify Service Level Indicators (SLIs) that will align the team to meet the availability and latency objectives.

**Collaboration and Communication:**
- Know a domain really well and radiate that knowledge
- Perform and run blameless RCAs on incidents and outages aggressively looking for answers that will prevent the incident from ever happening again.

**Influence and Maturity:**
- Lead Production SREs and Junior Production SREs by setting the example.
- Show ownership of a major part of the infrastructure.
- Trusted to de-escalate conflicts inside the team

### Staff Site Reliability Engineer

**Technical:**
- Able to create innovative solutions that push MayaData’s technical abilities ahead of the curve
- Deep knowledge of Director and OpenEBS and 4 areas of expertise. Knowledge of each area of expertise enough to mentor and guide other team members in those areas.
- Contributes to MayaData codebases to resolve issues and add new functionality

**Execution:**
- Strives for automation either by coding it or by leading and influencing developers to build systems that are easy to run in production.
- Measure the risk of introduced features to plan ahead and improve the infrastructure.
- Proposes and drives architectural changes that affect the whole company to solve scaling and performance problems
- Leads significant project work for OKR level goals for the team

**Communication and Collaboration:**
- Works with engineers across the whole company influencing design to create features that will work well with SaaS and self hosted platforms
- Runs RCAs and epic level planning meetings to get meaningful work scheduled into the plan

**Influence and Maturity:**
- Writes in-depth documentation that shares knowledge and radiates OpenEBS and Director’s technical strengths
- Has a high level of self awareness
- Trusted to de-escalate conflicts inside and outside the team
- Routinely has an impact on the broader Engineering organization
- Helps to develop other team members in to senior levels and leaders in the team

### Engineering Fellow, Infrastructure
The Infrastructure Fellow embodies all the requirements of less senior roles on this page. In addition, the role is closely associated with Engineering Fellow role in our Development Department.
- Drive the technical strategy of of our MayaData Director and other Infrastructure
- Heavily influence the technical strategy of our open-source application maintained by our Development Department
- Make skill-gap recommendations for future hiring in Infrastructure and other departments
- Author technical vision artifacts with >1 year time horizon
- Assist teams throughout Engineering to interpret this vision into actionable backlogs
- Help Engineering avoid the architecture "ivory tower"
- Spend time with customers to learn their needs
- Considered as an authority in all topics SRE by MayaData and its community. 


## Performance Indicators
Site Reliability Engineers have the following job-family performance indicators:
- Director and other sites Availability
- Director and other sites Performance
- Apdex and Error SLO per Service
- Mean Time to Detection
- Mean Time to Resolution
- Mean Time Between Failure
- Mean Time to Production
- Disaster Recovery Time to Recovery

## Hiring Process

All interviews are conducted using Zoom video conferencing software or in person. To learn more about someone conducting your interview, find their job title on our team page.

Please keep in mind that you can be declined at any stage of the process. You should consider each of the following bullets as though the words, "If selected" precedes them.
- You will receive a technical questionnaire to complete.
- You will be invited to schedule a 30 minute screening call.
- You will discuss your technical skills for 60 minutes with a member of the Reliability Engineering team.
- You will have 2-3, 45 minute team interviews with at least one Site Reliability Engineer.
- You will talk for 60 minutes with a Reliability Engineering hiring manager.

It's possible you may have additional 60 minute interviews with either the Director of Infrastructure Engineering, the Director of Engineering, or both.

If approved, you will subsequently be made an offer.

Additional details about our process can be found on our [hiring page](https://github.com/mayadata-io/culture/blob/master/process/hiring.md).

We are an equal opportunity employer and value diversity and inclusion at our company. We do not discriminate on the basis of race, religion, color, national origin, gender, sexual orientation, age, marital status, veteran status, or disability status.
