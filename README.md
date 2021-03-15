This repository contains the various MayaData Culture Guides/Handbooks and is the central repository of guidance for how we run the company. As part of our value of being transparent, our handbook published in this repository is open to the world. We welcome feedback. Please make a merge request to suggest improvements or add clarifications. If your question is not covered here, please use issues to ask questions.

## MayaData -- The Purpose

MayaData evolves around these few things:

- We build open source container attached storage.
- Container attached storage is per workload cloud-native storage that unlocks the productivity of these small teams; we sometimes think of it as DevOps friendly storage.
- Cloud-native is an approach to building and operating software that has certain basic principles that are closely related to DevOps.

It is incumbent upon everyone that works at MayaData to understand the above. That sounds simple -- it is only three things after all -- but when you dig into the definition of Container Attached Storage and thereby start searching for definitions of cloud-native and DevOps you can easily find yourself understanding concepts at a high level but missing the essence of them if you have not spent a lot of time with SRE and infrastructure teams to actually see how they operate.

Only our curiosity and empathy can save us here.  We must try to really understand what it is like to be our target persona -- Kubernetes SREs whether workload Kubernetes SREs or platform Kubernetes SREs; as an aside I believe we do much better for the former than for the latter which makes a certain amount of sense since workload Kubernetes SREs are closer to developers and the latter, platform SREs, are typically much more senior in the organization and focus on outcomes and operations and overall operational architecture as opposed to writing and running components. Product management and a (soon to be) great process or even a driven set of founders cannot substitute for our own empathy and understanding of the experience of our users. I’ve tried to emphasize this repeatedly, at one point making the perhaps hyperbolic statement that “we are all in product management”. The context for that statement was the above train of thought; without empathy for our users, we are doomed, or at least we are never going to be better than average and that would be a shame.

## MayaData Vision & Guiding Principles

Our north star remains **Data Agility** -- this is our vision and as such, it is aspirational which means that by design it is not something that appears in an immediate backlog. Data Agility refers to a future in which small teams innovate in building data-centric applications free from all sorts of nasty technical and organizational dependencies that historically have slowed them down. These include:

- Shared everything storage -- your requirements conflict w/ my requirements and we share a massive blast radius beyond our control

- Cloud lock in -- teams that rely on being spoon-fed by a particular cloud eventually end up being beaten by teams that are more able to select best of breed components from the clouds or from on-premise systems

- Central DB as a service that cannot be fully configured for a particular use; data mesh is a pattern that is supplanting the one DB to rule them all of the past

- Monolithic architectures that require the software to be released at best quarterly as opposed to minute by minute in a high performing organization

Here are a few practical implications for the design of our software and services that we may not have fully embraced in the past:

- *Automation is fundamental*: human interaction to tweak the settings means treating the containers as pets, not cattle.  That is an anti-pattern not consistent w/ cloud-native and Container Attached Storage.

- *Design for failure*:  Kubernetes and the cloud-native pattern assumes that everything will fail at some point. Chaos engineering such as the Litmus Chaos project we started and developed into a viable project enforces the need to design for failure by creating failures in systems.

- *GitOps*: Building off the importance of automation - the desired state of the environment is in the repository, i.e. GitOps is fundamental.

- *Loosely Coupled* may be the two most important words in [the CNCF’s definition of cloud native](https://github.com/cncf/toc/blob/main/DEFINITION.md). The need for loose coupling is one reason why our users like Steven Bower do not want to use shared storage. One video we have in the welcome and onboarding slides is [this interview with Steven](https://www.youtube.com/watch?v=z_LbRfDKPvE).

- *APIs and Declarative approach*: Loosely coupled and the existence of many sub-components suggests there are clear APIs including within the product and typically declarative approaches are used

- *Cloud operations including auto-scaling*: Cloud-native also tends to imply cloud scalability - the ability to scale UP and scale DOWN.

We will know we are succeeding in enabling our personas when a standard user of Kubernetes can grab OpenEBS and:

- *grok it* -- what it is supposed to do, how it is designed, how it is explained

- and *operate it* -- knowing that it will behave in a cloud-native or container attached storage way

…while the Kubernetes SREs within the Platform Team can support the use of OpenEBS at scale because they will be able to do their job. We have more work to do here in defining what these platform teams require -- thankfully we are in frequent contact with them at places such as Bloomberg, Flipkart and Optoro. 

Last but certainly not least -- we are working with data and increasingly important data that needs to be secured at least for some period of time.  We must avoid losing data, understanding that solutions such as flavors of OpenEBS LocalPV themselves by design do nothing to secure the data.  Remember the old saying, when our users lose their data they typically lose their jobs.

As a final thought, our technology strategy can be described as **giving freedom to the developers and the workload SREs** while selling control and operability at scale to the enterprise and platform SREs.  We believe in open source as a far better way to get more customers to pay us than traditional, expensive, much much slower to scale direct sales only approaches.  That said if and when appropriate, aspects of our software to be used by large enterprises in particular, as well as future SaaS editions, would not necessarily be open source.  We resolve such questions by looking at our north star -- Data Agility -- and our core values first and then secondarily by what would be good for immediate revenues and other considerations. 

## What is Culture

*Culture is a framework that is used for day-to-day interactions and decision making. When in conflict, the culture established and accepted is used to resolve differences.*

### Why are we writing this document?

Culture can be a secret ingredient that increases user adoption, product quality, employee engagement and well being. By writing down our shared assumptions and aspirations about our culture, we hope to improve and sustain our culture as our company grows and transforms to better address user needs.

History shows that employees either leave or really invest their best selves into organizations depending on the culture. Our values help us to prevent the [five dysfunctions](https://en.wikipedia.org/wiki/The_Five_Dysfunctions_of_a_Team#Summary).
- Absence of trust (unwilling to be vulnerable within the group) => prevented by people first, specifically kindness
- Fear of conflict (seeking artificial harmony over constructive passionate debate) => prevented by openness, specifically directness
- Lack of commitment (feigning buy-in for group decisions creates ambiguity throughout the organization) => prevented by openness, specifically directness
- Avoidance of accountability (ducking the responsibility to call peers on counterproductive behavior which sets low standards) => prevented by winning, and openness
- Inattention to results (focusing on personal success, status and ego before team success) => prevented by people first and winning

### Our Mission

We want MayaData to be the preferred place to work for engineers, computer scientists, community advocates and others that believe in our company mission to limit cloud lock-in while providing higher levels of control of the data layer to DevOps teams. We recognize that in order to achieve our mission we have to be the _**best team**_ possible at _**building**_ and _**running**_ the _**right software**_ based solutions to our customer’s problems. We commit to always working to improve MayaData - and ourselves - to delight our customers. Our culture plays a key role in achieving this mission.

Specifically:
- When we talk about the _**best team possible**_ we emphasize that we expect high degrees of collaboration and teamwork; if you cannot work with a team with multiple cultures with high degrees of sensitivity then we are likely not the right place for you. We seek to be the preferred employer for the best contributors in Bangalore and other markets in which we hire.
- When we talk about _**building software**_ we emphasize that we focus on the productivity of our engineering teams and will be relentless in improving their ability to respond to customers quickly. We will aggressively seek to continuously improve our CI/CD and operations abilities for example.
- When we talk about _**running software**_ we emphasize a DevOps approach so that if you write the code, you support the customers and you lead efforts to fix any bugs.
- When we talk about _**the right software**_ we emphasize listening to users. We believe everyone at MayaData can learn from users and customers and that the best learning comes from users actually using software as opposed to simply talking about it. In order to learn from internal users, we believe in *dog fooding* which is the practice by which we will always use our own software if it is at all applicable to our use cases. Development environments, staging, and CI/CD and of course operations should all be based on OpenEBS and OpenEBS Director.

### Our Values

We stand by our [PLOW values](/plow/plow.md). They empower each of us to determine what to do without asking our manager.

## Additional Resources

This site expands the [MayaData secret plan for world domination](https://medium.com/mayadata/mayadatas-secret-5-step-plan-for-world-domination-3c02ac8b097a) and converts the plan into a culture we aspire to achieve as well as concrete actions to implement and measure adoption of the culture.

We have also covered topic of the Container Attached Storage multiple times including:

- Back in 2018:  [Container Attached Storage: a Primer](https://www.cncf.io/blog/2018/04/19/container-attached-storage-a-primer/)
- Updated in the Fall of 2020: [Container Attached Storage is Cloud Native Storage (CAS)](https://www.cncf.io/blog/2020/09/22/container-attached-storage-is-cloud-native-storage-cas/)

And others such as the New Stack in a series sponsored by the CNCF have also written about [the concept of Container Attached Storage](https://thenewstack.io/how-openebs-brings-container-attached-storage-to-kubernetes/).

### Credits and Inspiration

[GitLab Handbook](https://about.gitlab.com/handbook/) is a true source of inspiration for anyone praticing the Open Culture. We have developed our handbook by our own experiences, as well as those mentioned in the GitLab handbook which directly reflect our [PLOW culture](/plow/plow.md). Another great source of inspiration and a must read are [The Open Organization](https://opensource.com/open-organization/resources/book-series) book series by Jim Whitehurst. On similar note, are the [Amazon’s Leadership Principles](https://www.amazon.jobs/en/principles).

Excellent inspiration for building great organizations are also [An Everyone Culture: Becoming a Deliberately Developmental Organization](https://www.amazon.com/Everyone-Culture-Deliberately-Developmental-Organization/dp/1625278624/) by Lisa Laskow Lahey, Robert Kegan and [Principles: Life and Work](https://www.amazon.com/Principles-Life-Work-Ray-Dalio/dp/1501124021/) by Ray Dalio.

Many of us read the book [Accelerate](https://www.amazon.com/Accelerate-Software-Performing-Technology-Organizations/dp/1942788339/) -- and we discussed it as a company a couple of times. It remains one of those books that we would welcome anyone on the team buying and expensing. Others along these lines are the [Phoenix project](https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business/dp/1942788290/) and [The DevOps Handbook](https://www.amazon.com/DevOps-Handbook-World-Class-Reliability-Organizations/dp/1942788002/).
