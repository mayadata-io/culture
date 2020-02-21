[[TOC]]

# Introduction

This document describes MayaData’s Customer Success Advocacy Team/Organization structure and processes to achieve customer success as we expand product offerings and grow our customers. 

The content in this document is derived from past experiences as well as learning from the following online resources:

* [https://www.helpscout.com/helpu/customer-support-department/](https://www.helpscout.com/helpu/customer-support-department/)
* [https://www.zendesk.com/resources/structure-customer-support-organization/](https://www.zendesk.com/resources/structure-customer-support-organization/)
* [https://www.mmcventures.com/wp-content/uploads/2018/05/MMC-Ventures-Customer-Service-Playbook-single-pages.pdf](https://www.mmcventures.com/wp-content/uploads/2018/05/MMC-Ventures-Customer-Service-Playbook-single-pages.pdf)

# Customer Success with MayaData

The PLOW culture at MayaData emphasizes that entire company MUST empathise with the Customer and make the Customer win within his/her Organization.  

The single most important objective that the whole company strives for is to **_Deliver Data Agility - Free DevOps and Kubernetes from storage constraints using OpenEBS, validate with Litmus by chaos engineering and monitor with MayaOnline_***.*

Our design philosophy is to deliver radically simple solutions that are open source based that enable developers and DevOps end user self service success.  We then sell solutions that wrap around these solutions to enable enterprises to control, manage, and scale their operations.  

MayaData has chosen Chat as the primary mode of customer support, since Chat implicitly sets the expectations for a shorter response time compared to emails and also maintains a record of the interactions as opposed to Phone conversations. MayaData sets the bar for quick response very high compared to other companies - at less than 15 minutes.   Our goal is to be a trusted partner to our users - **_whether they are paid customer or community user_** - as they seek to achieve data agility.  Through this trusted relationship we can out learn alternatives while also building customer trust and loyalty.

In addition to Chat (Slack), MayaData customer support team also uses ZenDesk for Ticketing and tracking the SLA.

To achieve our rapid initial response SLA of less than 15 minutes, MayaData customer success organization is spread around the world - with at least one Tier 1 personnel on staff during work hours North America, Europe, and Asia - so that users have access to customer success available 24 x 7.  A detailed schedule (*see Appendix : Support Shift Schedule* ) is published to maintain ownership of quick response. As the volume of the requests increase, the number of personnel available will be reassessed. 

*Tier 1 customer success personnel are arguably the most important in MayaData when it comes to building a trusted relationship with end users and customers; these trusted relationships will, over time, result in customer growth and customer word of mouth which are the engines upon which the growth of MayaData is being built.*

Tier 1 professionals listen to the Customer query or issue, gather additional information about the issue and acknowledge that they have understood there is a problem.The tone of the Tier 1 personnel needs to be welcoming and empathizing - rather than instructive or dismissive. Tier 1 personnel must and will have access to all the information and necessary team and resources of MayaData to provide responses to the Customer. The first person to interact with the customer is accountable for making sure the Customer issue is resolved and issue and resolution are well documented in the Knowledge base for future references.  Moreover, at MayaData customer success is responsible for user growth -> as such with each communication more information about the needs of the users can and should be recorded; such information can be tremendously valuable in shifting the relationship from a *reactive* one - in which MayaData *waits* to see if there are issues - to a *proactive* one, in which MayaData is actively working with users to advise them on ways to achieve their desired outcomes.  

The day to day activities of Tier 1 personnel include interacting with users, recording the issues as they occur, identifying opportunities to grow customer usage, and providing feedback to product management to prioritize product, solution and partnership development.  

When recording issues, Tier 1 personnel triage incoming tickets into the following: 

* Sev 0 : Data is lost or compromised. Nodes or Pods are getting crashed.
* Sev 1 : Data is not accessible 
* Sev 2 : Operational Complexity 
* Sev 3 : New Features or Enhancements to existing features

Tier 2 and Tier 3 are engaged in case of Sev 0 and Sev 1 immediately for engineering debugging and/or hot patch application. Tier 1 plays an important role in reducing the volume of tickets requiring Tier 2 and Tier 3.  When a ticket reaches this level it means our product simply is not working as needed - users are unable to self sustain, have uncovered a bug or other operational issues, and may be at risk of not becoming a reference.  

Product management and engineering are accountable for making sure, when Tier 2 and Tier 3 tickets are in progress, the entire organization need to be working on them to resolve them ASAP both to help particular customers and to insure that we improve the product, solutions, and partnerships and even marketing so such issues are avoided in the future.

OpenEBS products are available in Community and Enterprise editions. The Community Edition is targeted towards tech savvy DevOps personnel who would like to try out and contribute back to the product. Taking the community edition to production requires DevOps to write their own tooling to help with alerting and troubleshooting. 

Enterprise Edition lags behind Community Edition in terms of releases/features, but is bundled with MayaOnline and required support tools that greatly simplify the tasks performed by Customers. The Enterprise Edition involves qualifying the product with the supported platforms using automated e2e via Litmus.

The products are architected and engineered in such a way that:

* Potential user configuration or setup issues are identified, validated and administrator/users are notified
* When issues do happen, they can be easily troubleshooted and fixes can be patched immediately to reduce any downtime experienced by the users.

We need customers to trust us with their data and we take full responsibility to ensure that MayaData products and support services are well equipped to provide a resolution to the Sev 0 and Sev 1 issues within 48 hours - with either a workaround or hot patch. 

As we interact with customers, we also need to be cognizant of two challenging situations: 

* Responding to an unsupported feature. In this case, acknowledge that the feature is currently not planned for the road map and include the product manager and (cc: sales) representative for further discussions. The product manager will interact with the customer to identify if the feature is really required, is there an alternative solution and also discuss on the priority compared to other features that are being worked on for the customer. 
* Responding to disagreements about the problem or root cause. It is very common that the new product is perceived as the cause for all the problems and especially storage is to blame for everything. Be sensitive that customer has a real issue and in his attempt to find the answers is hoping that the issue lies with the storage and it can be resolved. Always respond to such situations with tangible data or facts. Work towards enhancing the product and tools that can isolate the issue and present data that can be easily understood by the customer to look into the right direction for resolving the issue. 

A great customer service can only be provided when the entire organization backs the Customer Success team and the Customer Success team feels ethically responsible for making the customer win. 

We as Customer Success team needs to imbibe a culture where:

* We actively pursue users engaged with our products, to understand how they are using our product, what features are they liking and disliking, and reach out to them with information on how they can benefit by using best practices. 
* We focus on solving user problems - the problems that the user has that led them to use OpenEBS and MayaData in the first place
* We hold ourselves accountable to meticulously follow the process including opening and closing tickets in order to capture learning and provide a record of usage
* We hold each other accountable for making continuous progress on the open tickets 
* We are constantly improving the process for achieving greater success including improving their own worklife (see DevOps philosophy)
* We understand our design philosophy - enabling end users to succeed while also allowing enterprises to control, scale and manage their data layer operations with the help of OpenEBS and MayaData

Customer Success Channels 

Helpscout provides a good summary of the various Customer Success channels with their pros and cons, which also align with the thought process that has led to MayaData Customer Success being offered through Slack, instead of Phone 

*Small teams can’t necessarily provide consistently great Customer Success across all possible channels 24/7. It’s far better to provide quality customer Customer Success on a few channels than to spread your team too thin and give inconsistent service.*

*Live chat**—A good mix between email and phone Customer Success — in some cases the "best of" both email and phone. Pro: Makes back-and-forth less cumbersome by allowing Customer Success teams to hash out issues in real-time without the necessity for long phone conversations. Con: Customer expectations for response time are higher than email, so it can still require more people.*

*Phone**—Pro: Allows for direct conversation in real time and remains very popular with older generations. Con: Phone Customer Success can be very time consuming (and costly), especially for smaller teams.*

*Email**—The most widely used channel by far. Pro: It is conversational, asynchronous, and an excellent record of past discussion. Con: Email can be frustrating if there is a lot of back and forth required.*

*Knowledge base & self service tools**—Pro: An excellent way to scale your customer service efficiently, by enabling your customers to help themselves. They take some initial investment, but they’re well worth it in the long run for the time they save your Customer Success team.*

*Forums**—Pro: These allow your community help each other, which can save you time and resources. Con: They require diligent monitoring to temper trolls and ensure customer questions get answered.*

*Social media**—Pro: Facilitates conversation around your product or service. Con: It’s a very public space, and people typically expect an immediate response on social media, so consider that when you decide which platforms (and how many) to Customer Success.*

MayaData will continue its Customer Interactions via Slack till 2019-Q2, since it falls under the small teams that is striving for great customer service. The Customer Support type and channels are categorized as follows:

* Community Customer Support is provided via Slack (openebs-users#general) channel with an SLA of 3 hours for initial response. Most of the queries are responded to by the Tier 1 personnel and in cases where the Engineering help is required, the users are requested to raise an GitHub issue (or an issue is raised for the user), where further workaround or solution are provided.
* Evaluation Customer Support is provided via Slack (openebs-users#company) dedicated channel with an SLA of 1 hour for initial response. In addition to the Tier 1 personnel helping with the issues, the Tier 2 and Tier 3 (Engineering) teams also directly interact with the user to resolve the issue. For Sev 0 and Sev 1 issues, the Tier 2 and Tier 3 teams will setup Live Zoom sessions to troubleshoot and provide resolution.
* Customer Support is similar to the Evaluation Customer Support channels and SLA and additionally includes the feature to track the tickets via Self Service Portal - ZenDesk. The tickets can be raised directly via MayaOnline.
* Premium Customer Support- has all the features of the Customer Support and additionally will provide access to a Phone contact that can reduce the FRT SLA to less than 5 mins for Sev 0 and Sev 1 issues

Email channels will be limited to sales and notifications regarding security vulnerabilities, hot patches, and new releases.

Knowledge Base will be integrated with ZenDesk and accessible via Customer Login. There is also a community based Knowledge Base that is available on Stack Overflow, GitHub etc., The Tier 1 personnel will help building the Knowledge base as tickets are resolved. 


# Customer Success Team Structure

The Customer Success  teams directly interact with customers to help them quickly solve their problems and ensure customer satisfaction remains high. Some of the essential skills required by Customer Success team:

* Empathetic: People in customer service roles should genuinely want to help other people. That desire begins with empathy: the willingness to understand another person’s experience and see it through their eyes.  One proof of empathy is the ability to express the users needs in one’s own words.  

* Internet savvy: The internet and mobile computing provide us with more ways than ever to communicate with each other. We refer to these as channels, and we often provide customer service simultaneously on many different channels

* Strong communicator: This job is about communicating with other people. Advocates need to communicate well both verbally and in writing. Communication is about listening, then clearly articulating ideas and information in an authentic way.

* Master of simplicity: When a customer makes the effort to reach out and ask for help, it’s the Advocate’s job to quickly assess the problem, sort it all out, and then present the customer with the simplest answer possible.

* Growth mindset: Products, technology, and policies will change over time, and your Advocates will need to change with them. Look for people who have demonstrated a drive for learning and growing.

Customer Success teams directly report to the *Vice President of Customer Success, *who ensures that the Customer Success teams are highly motivated and aligned to the Organizational goals. Within the Customer Success Team, levels of seniority are defined that gives people who are happy in a customer-facing Customer Success role the opportunity to demonstrate peer leadership and gain status, while staying in a job that they love.

## Tier 0, making the most of self-service

This is the self-service tier: the support available to customers that does not require directly interacting with a customer advocate. This includes the knowledge base available in online Help Center: the product training that is available to customers, as well as assistance that is available in the product’s user interface.

Tier 0 isn’t a staffed team, it’s an initiative to better contribute to and manage self-service as a Customer Success channel; to better handle an ever-increasing amount of incoming support  requests that can be easily answered with these self-help resources. 

There are two goals for Tier 0. The first is to practice Knowledge-centered Customer Success (KCS), which means that Customer Success Representatives are both generating and sharing knowledge-base content (internally and with customers). The second goal is to devise ways to help customers discover and use that self-help content. An example of this is to use proactive support to spot an issue that a customer is having or is about to have, then proactively create a ticket that contains a link to the knowledge-base article that will help them resolve it themselves. 

## Tier 1 is for general product Customer Success

This includes things like helping customers understanding the OpenEBS concepts and how it works, pointing in the right direction with the help of Documentation or KB articles, helping them navigate through MayaOnline. 

Tier 1 is also the first point of contact for incoming Customer issues. This is where all incoming tickets are triaged and then routed to the appropriate team or tier. The Tier 1 team also handles all incoming chats and phone calls. 

Experienced Tier 1 Advocates take turns triaging tickets and determining how they should be assigned based on complexity, which is defined by the time needed to resolve the issue. Customer Success issues that are assigned to Tier 1 are expected to take 15 minutes or less to resolve. If a Customer Success issue is more complex and requires more time to resolve, it’s assigned to Tier 2.

Tier 1 includes these Customer Advocate roles:

* Associate Customer Advocate
    * This is the team’s entry-level role. We look for people with potential, who have 0-2 years of experience helping customers in some capacity, and who possess essential customer service skills. 
    * Associates are in training and need guidance to perform at the standard level set for customer advocates. We set a target for tickets solved per day and expect an overall customer satisfaction (CSAT) rating of 90%. Associates are usually in this role for at least 3 months before becoming full-fledged Advocates
    * This team is well versed with the concepts and has undergone the OpenEBS training and workshop. 

* Customer Advocate
    * Advocates are well-trained and can handle most types of general support issues; therefore, they don’t wait for tickets that they understand and feel comfortable to respond. Their performance is measured by the number of tickets they solve per day and by their CSAT rating, which should be at least 95%.
    * In this role, the Advocate has gained experience in installing the OpenEBS product and connecting them to MayaOnline. Has the ability to determine the components that are potentially causing an issue. 
    * The Advocates are comfortable editing and updating the OpenEBS and MayaOnline Documents based on the learning by interacting with the users. 

* Sr. Customer Advocate
    * A promotion to Senior is possible after about 9 months of successfully working as an Advocate. Advocates must demonstrate that they can proactively identify problem areas and mentor and train other customer advocates on how to solve more difficult tickets. 
    * A Senior’s performance should be above the standard, and they should also have an average CSAT rating of 96%. They often specialize in one or more product areas and are considered experts in those areas. 
    * Senior Advocates are responsible for identifying the issues are causing pain to the customers and are causing the customers to drop off. The issues need to be escalated to the Customer Success Team. 

*"I think sometimes Tier 1 Customer Success is overlooked. Having a Tier 1 title doesn’t mean that you’re the lower end of Customer Success. For me, it’s one of the most difficult groups in Customer Success. You need to learn the entire product as a whole because you get all sorts of different tickets in the queue. I’ve worked on other tiers, and the tickets are increasingly difficult. But the way you interact with customers tends to be more personal at Tier 1."*

## Tier 2 is for technical Customer Success

This team often helps customers with issues that involve aspects of the product that are requires knowledge of code. The issues can’t be debugged or resolved by using the CLI or MayaOnline. Tier 2 is often members of the engineering team - development, testing or solutions, depending on whether the issue is related to core product, application workload or integrated platforms..

The tickets that are assigned to this team are expected to take 30 minutes or less to resolve. If a Customer Success issue can’t be handled in that amount of time, it’s escalated to the Tier 3 team. 

Tier 2 includes these roles:

* Technical Customer Success Engineer:  Typically these engineers have worked on this product area and have contributed in terms of fixing bugs or adding small features. These engineers are familiar with the logs and the code structure. Typically, Advocates also can move into the Technical Customer Success Engineer role after having been an Advocate for at least one year. Of course, they also need to have developed in-depth technical knowledge about one or more product areas. Like Advocates, Customer Success Engineers have a target for tickets solved per day (a lower number than for Advocates because the issues they work on are more complex) and an average CSAT rating goal of 94%. 

* Sr. Technical Customer Success Engineer: A Senior has usually mastered multiple product areas, is capable of leading productivity improvements, and defines best practices within those product areas. They’re recognized as a point of contact for their product areas across the entire customer service organization, and they collaborate closely with the Product Management teams to represent the needs of customers. They have a target for tickets solved per day and need to achieve an average CSAT rating of 95%. 

OpenEBS and MayaOnline are very vast in terms of complexity and can be divided into sub areas - like Provisioning, Upgrades, Jiva, cStor, MO Logging, MO Topology etc., There will be a chart available that can showcase the Engineers and their expert levels in each of the sub areas. As members of Tier 2 specialized squads, Engineers develop product expertise by interacting with the uses in their current area of focus. The expertise that they develop helps the organization handle complexity and resolve issues more quickly.  Tier 2 Customer Success Engineers are expected to (and want to) cycle through multiple product areas. This gives them the opportunity to master all the areas of our products. Doing so also helps prepare them for a move into Tier 3. 

## Tier 3 is for advanced technical Customer Success and engineering escalations.

*The team has to have persistence and patience; a lot of the issues take a long time. We have to have a broad scope—to have wide knowledge across products, but also the ability to be very technical. Also, it takes teamwork, jumping in to help each other and to form close-knit relationships.*

*What I like about Customer Success engineering is that I can help customers, work on projects with engineering, and focus on really difficult questions. In other tiers of Customer Success, maybe you have to focus on helping more customers in less time. But in Customer Success engineering, you basically have to do as much as you can, going above and beyond to help. There’s nowhere else to go after Customer Success engineering, so you’re the last person the customer is going to talk to.*

This team can get both Sev 0 and 1 escalated tickets or Sev 2 and 3 tickets that require product or strategy change to resolve. 

When Sev 0 or 1 tickets are received, the members of this team will form a tiger team that is fully dedicated to resolve and help the customer get out of the issue. All other tasks being performed by the tiger team will be kept aside. 

If Sev 2 or 3 tickets are received, these tickets have no time limit for resolution; they take as long as they as take to resolve. They’re often issues that are hard to replicate and may be dependent on products or infrastructure beyond our own products. However, with these tickets, this team members are expected to set the expectations with the customer and continuously keep the customer apprised of the progress and blockers. 

This team comprises of the Technical Architects in their respective product areas. 

* Customer Success Technical Architects
    * Customer Success Technical Architects have mastered multiple parts of the product (because they’ve participated in Tier 2 squads) and, as liaisons to the Product Management and Development teams, help each of those teams understand where the product can be improved and how
    * The difference between a Customer Success Engineer and an Architect is experience, subject matter expertise and technical mastery, and their influence in the organization. They’re expected to provide guidance and best practices for providing excelling support for their areas of product expertise. They are trainers and mentors. 
    * Technical Architects have a daily ticket solve target and an average CSAT rating goal of 90%

* Sr. Customer Success Technical Architects
    * At this level, Seniors are excellent at communicating complex customer issues to software development teams and can make suggestions for improving the product and influencing the product roadmap.  
    * They also interact directly with VIP customers to provide a high-touch technical support experience when needed.
    * Sr. Technical Architects have a daily ticket solve target and an average CSAT rating goal of 92%.

## Management Team

Customer Success Management teams are responsible for making sure that the organization delivers the kind of Customer Success that we promise to our customers. Doing that requires using resources wisely, staying on top of key customer service performance metrics, being an effective people manager, and constantly adapting to change.

To help to rise to that challenge, the Customer Success Management team believes that you need to create a great overall Customer Success experience by being as concerned with the Customer Success Teams experience as you are with the customer experience. In short, happy teams equals happy customers.

MayaData has a flat people hierarchy, the Customer Success team is managed by Director or VP of Customer Success. The skills and goals of this role are:

* Require strong people and project management skills. They need to build relationships, manage performance, and deliver on their commitments.
* Are concerned with many other essential customer service metrics such as first reply time, first contact resolution, handle time, and so on. 
* They are strong influencers across the organization and company and often work with the Sales team and VIP customers. 
* This role believes that the best customer experience is achieved when you also focus on the agent experience. Combined, the two create the Customer Success experience.
* CSAT and ESAT surveys are taken to address concerns from both customers and employees. 

Key Skills are:

* Communication - You communicate well by building relationships based on trust and respect.
* Direction setting - Building healthy relationships helps you set direction by telling the story of where you’re going and why
* Motivating and recognizing - Building healthy relationships helps you set direction by telling the story of where you’re going and why
* Change management and removing roadblocks - You manage change effectively by using critical thinking to re-design better processes, get buy-in, train people, align everyone’s behavior to those new processes.
* Conflict management, feedback, and development - You handle difficult conflicts on the team by giving tough, fair, but direct feedback. 
* Hiring, onboarding, and diversity - Build your team with a lens on diversity and inclusion by hiring great talent and onboarding them well. 

# Supporting Customer Success Team

## Planning the first few weeks. 

In the first week of onboarding the Customer Success personnel, carry out the following checklist:

* Assign a Buddy who can help with the on-boarding process and is the go-to person for any clarifications required by the new joinee.
* Review the team structure - schedule meetings with the leads of various teams to get an idea of what everyone does
* Provide them with the required training and exercise to get familiar with the product and solutions.
* Provide access to the various tools. 
* Help setup the Goals and Objectives and help them track their performance via (Key Performance Indicators)KPIs. Help them understand the Growth path with in the organization. 
* Host regular training sessions and educate on the best practices.
* Mentor them to take ownership with the day-to-day operations. 
* Help them embrace and strive for continuous improvements in customer Customer Success to become more efficient in process (or internal operations).  


Finally—and most importantly—train your techs to manage client expectations and give confirmations. When a client asks for a status update, it means expectations weren't met. Clients like to be contacted, so don’t forget: When in doubt, reach out!

## Knowledge Base

Developing a knowledge base is time consuming, no doubt. But your investment will be rewarded tenfold when your customers can find answers on their own, lessening the strain on your Customer Success team. They also allow for faster onboarding and greater consistency of Customer Success.

A knowledge base will also save time when responding to common customer questions. Not only is the customer service team able to quickly answer the question, it also helps the customer learn that there is a knowledge base available to them at any time.

Most help desk software offers [knowledge base reporting](https://www.helpscout.com/help-desk-software/reports/#docs-report), a valuable tool for successfully scaling your Customer Success. It will show you where your customers are getting stuck, what documents need updating or adding, and how to prioritize product improvements.

Internally, taking the time to write down how certain issues are handled and how to use different tools will let new team members grow their skills without needing to disrupt the existing team.

You don’t need to do this all at once. You can build your knowledge base as you go, either as demand arises or by working from a Customer Success content calendar. We shared some great examples of [knowledge base pages](https://www.helpscout.com/helpu/knowledge-base-examples/) on our blog if you’re looking for some inspiration.

## Integrate Customer Success into your product and company

No matter how great your frontline staff is, their experience is inevitably shaped by what the rest of the company does, too.

The goal of a customer-focused company should be to build in systems across teams that Customer Success great service so that delighting customers is more of an automatic outcome of doing business, rather than an occasional, heroic feat. Customer Success managers can take these steps to build systems into their teams:

* Push decision making to the front lines Don’t make your Customer Success team ask for permission to commit to solutions that can delight the customers. Give them tools and information to make better decisions, and back them up on it.
* Automate customer-friendly processes This ensures a more consistent customer experience and requires fewer decisions, which saves time for everyone involved.
* Create feedback loops Actionable input from customers needs to make it past Customer Success to be useful. Make sure you are providing a framework for your Customer Success team to share customer feedback with your product team and others.
* Customer Success your team Your customer Customer Success team is fielding the good, the bad and the ugly day in and day out, so treat them with the respect they deserve. They are also the voice of your customer, so involve them in product and strategy meetings. Celebrate their successes, and hold them accountable for their work.

## Customer Success Operations

The Customer Success Operations team (Customer SuccessOps) helps the teams that directly interact with and assist customers (the Tier 1, 2, and 3 teams). They do this by defining and streamlining processes and workflows, building tools to help make delivering Customer Success easier, providing education and training to Advocates, and evaluating and making sense of all the Customer Success data that’s available to help assess the organization’s performance and just how well they serve their customers.

* Support Management Specialists  - As an example, a Specialist may be charged with monitoring key customer service performance metrics and reporting that data to the management team. Another Specialist may be helping to build the internal knowledge base and Advocate training materials. Another example is to ensure surveys are sent and data collected from Customers and Employees.

* Tool Developers - Tools Developers are software developers who build custom tools that help the team deliver better customer service. For example, this team can develop log collection from customer or write tools that can help the customers check the health of their system. The other set of tools could also be related to collecting the metrics that can help with measuring the success rate of the teams. Required experience here really depends on your specific situation, what tools you’re using, how much customization you need, and the complexity involved in building those customizations. 

# Customer Success Tools

## Customer Ticket tracking software

ZenDesk is selected as the choice of Customer Ticketing Software. (The alternative considered with HubSpot HelpDesk and Rally - the two other tools used within the MayaData organization. Both of the alternate tools didn’t provide an option of letting the customers login to the ticketing tool and check on the status of their tickets.)

ZenDesk allows for Agents and Customers. To limit the cost of the tool, only the Customer Success Management team is added as Agents to track the tickets. The Customer Success Team (comprising of the rest of the organization) are added as Customers.

An organization called "Community" is created for tracking the tickets coming from the users on the Slack channel. For customers interested in evaluation or paid, the customer’s commany is added an organization. The MayaData employees are part of both the Community and the Customers Organization and will have the ability to update the Tickets.

The severity of the tickets is assigned based on the criteria defined above for Sev 0 to Sev 3 - using the ZenDesk Priority Feature. The tickets are further classified in the product areas.

The ticket state indicates the current engagement status:

* New: Yet to respond to the customer
* Open: More details are being gathered and the customer still has the issue. 
* Hold: The issue requires a product or documentation change. The customer is notified of the workaround. The ticket is linked either to the OpenSource (github) or Closed Source (Rally) work item.
* Pending: The issue has been fixed and customers can apply the change. 
* Resolved: The customer has confirmed that the issue has been fixed. 

## Internal tools and systems

Software tools built in-house are often the back alleys of a company, given little attention or effort and built by people hurrying to get back to the "fun" work.

Customer service teams are often heavily dependent on internal systems like custom database searches, configuration pages, and logging systems to access customer information, fix issues, and report back to the company. If you truly value their contribution, spend some time and effort to make those tools efficient and, if not attractive, then at least not actively painful to use.

## Personal tools

Allowing your customer team some flexibility in which tools they use to get their job done will help them be more effective. Help Scout, Basecamp, and other forward-thinking companies provide budgets for individuals to purchase small pieces of software and hardware that suit their requirements. Leave your team with flexibility everywhere you can, because you will gain back much more than it costs you

# Customer Success Metrics

## Customer Onboarding

The following metrics will be used to determine the funnel and the conversion rate. The metrics are collected weekly to track the progress.

* Number of users visiting Marketing sites
* Number of users visiting the openebs - code and docs sites
* Number of docker pull, cluster call home metrics
* Number of users visiting the MayaOnline 
* Number of users registering with MayaOnline
* Number of users connecting the clusters to MayaOnline
* Average time of the clusters in MayaOnline by the users. 
* Number of users requesting for Evaluation
* Number of users subscribing 
* Number of users renewing the subscriptions

## Feel the Pulse of Customers. Happiness Index. 

*Are our customers satisfied? What can we improve?*

Survey your clients and get a reading on how satisfied they are. Hearing directly from your customers can help paint a picture that tickets alone may not be able to provide. Reach out to the customers with different survey depending on their engagement. 

* Idle Customers - who have signed up but have not raised a ticket or connected their clusters 
* Raised Tickets have been resolved. Reach out with a CAST survey to check for:
    * Satisfaction in terms of handling the issue
    * Suggestions for improvements in getting better experience. Can the docs, KB or the products be improved. 
    * Understand the use case at a broader sense. 
* Posting queries about the product or upgrade questions. Reach out with HXC survey checking with customers on:
    * Finding out how much value OpenEBS is adding to their DevOps tasks
    * What Problems it is helping solve
    * Check if they will become a reference user
    * Find out the pain points with OpenEBS
* Stopped being active. Reach out with Feedback survey to identify the reasons for moving away from OpenEBS.

## Ticket Analysis

Analyse the ZenDesk tickets, FullStory recording to identify:

* Documentation Improvements
* Common Product Issues - that are hindering adoption
* Time of Day or dates when the volumes of the tickets is more. Check if more team members need to be onboarded with Customer Advocacy. 
* Measure the SLA for different issues
* Follow up on the issues that have been resolved.

Chart out the plan and track the progress and measure the improvements. 

## Motivated Customer Success Team

*How are the individuals on the team performing and feeling? *

Conduct ESAT survey with the employees - that are both involved and not yet involved. Check on what hinders them from being effective in Customer Advocacy.

# Appendix

## Escalation Matrix

The customers can use the following Escalation Matrix:

* Report an issue via Slack or MayaOnline or via Email to ( [support@mayadata.io](mailto:support@mayadata.io) )
* Send an email to Support Leads in case there is no response to ( [support-leads@mayadata.io](mailto:support-leads@mayadata.io) ). The ZenDesk will be automatically setup SLA triggers for initial response. The customers are also provided with US 1800 Phone.

## Support Shift Schedule

As the current teams are located in California, Europe and India, ownership of engaging the community and the users is as follows:

<table>
  <tr>
    <td>PST</td>
    <td>IST</td>
    <td>CET</td>
    <td>Who’s supporting</td>
  </tr>
  <tr>
    <td>02:00 AM - 10:00 AM</td>
    <td>03:30 PM - 11:30 PM</td>
    <td>11:00 AM - 07:00 PM</td>
    <td>Europe* and India</td>
  </tr>
  <tr>
    <td>10:00 AM - 06:00 PM</td>
    <td>11:30 PM -07:30 AM</td>
    <td>07:00 PM - 03:00 AM</td>
    <td>US</td>
  </tr>
  <tr>
    <td>06:00 PM - 02:00 AM</td>
    <td>07:30 AM - 03-30 PM</td>
    <td>03:00 AM - 11:00 AM</td>
    <td>India</td>
  </tr>
</table>


At the moment, the Europe team is understaffed and hence the India team will help out. 

## CSAT Survey Template

* How did you find the interactions with the Engineer helping you resolve the issue?

## HXC Survey Template

* In what aspects of your Work has OpenEBS made significant difference?
* Who in your organization do you think is most benefited from OpenEBS?
* What improvements would you like to see in OpenEBS in the next 3 to 6 months?

## Lost Customer Feedback Template

* What were your biggest concerns with OpenEBS?

## ESAT Survey Template

* How many customers have you directly helped succeed in their job last quarter?
* What aspects of your work in the last quarter has helped customers perform their job better?
* Are you working on a feature that will help customers in the next 3 to 6 months? 
* What are your biggest challenges in helping customers succeed? 
* In what areas would you like to help customers succeed?
