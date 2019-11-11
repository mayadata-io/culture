User onboard audit
Purpose:

Onboarding users is critical for any business or community - and especially for a project such as OpenEBS and a company such as MayaData for a number of reasons including:
Limited time: Our users are busy - and they try us out typically on their own time to gain understanding and trust before using our software and software services at work
Product and brand promise:  OpenEBS is known as the easiest to use and deploy solution for turning Kubernetes itself into a data plane.  If this capability erodes then we violate our brand promise, and disappoint users and lose their trust.  
Self adoption model:  Unlike vendors selling technology into enterprises from a prior era - , our approach is similar to that of GitLab or Atlassian or PagerDuty or GitHub or countless others - our solution must be self adopted and used in production typically before we even speak to the user.  Our entire model, from IO in the user space to the branding of the Mule for the OpenSource community to the attributes we look for and reenforce in our team, is based on self adoption.  Without effective self adoption we have built the wrong company, team, product, brand and other investments and commitments.

In short, poor self adoption is an existential threat.

This narrative suggest an approach to ensuring that we continue to evolve in the direction of improved ease of self adoption via a rhythm of user onboard audits.  

Proposal:

With each monthly release we will convene a cross functional team - whose members will rotate as described below - in order to perform the self adoption audit.

The specifics of the self adoption audit will evolve with experience.  Each team and each sprint will add or subtract components as they feel reasonable.  

In all cases, the self adoption audit will highlight, document, and prioritize areas that could reasonably be assumed to impede the self adoption of our target persona - an engineer that understands enough about Kubernetes to have adopted it or to be running software in an environment based upon Kubernetes.  

The process should include everything from - how do they find out about OpenEBS and OpenEBS director to initial deployment on leading platforms to any necessary customization.  Each monthly effort and team can choose to explicitly focus on particular areas however all efforts and teams should deploy on AWS and OpenShift and D2IQ (subject to change).

The team should be comprised of engineering, product, marketing, and sales stakeholders.  Actual end users in the community and partners such as D2IQ can be incorporated if available as well.

While team members will inevitably be of different levels within MayaData, for the purposes of the monthly effort, the team should self organize.  Likely important roles that should be assumed include:
Process documentation - what are we going to do?  Where are we in our validation?  
Platform research - what are the likely issues we may encounter - what has changed in OpenShift, AWS, and D2IQ?
Naive user - who can free their mindsmind from all that they know about OpenEBS and actually do the work of trying out OpenEBS as if for the first time?
Results - what did we learn, how many attempts did we make, how long did it take us to achieve success?
Results integration - are all of our prioritized results on the backlog?  Are there any typos in the docs or improvements to Helm charts or other items that we can fix right away, without waiting for the next release?  Keep in mind that words such as docs and other instructions are often easier to change than code.

Implementation:

After review and improvement - this proposal should be implemented immediately.  The total duration of each audit should be part time effort for one week per month.  

The team may want to convene via a kick off meeting with a senior sponsor such as a founder or senior technical leader.  During this 60 minutes meeting the purpose will be reviewed and the organization of the effort will be agreed upon.  At least one member of the prior month user adoption audit will attend to answer any questions.  

The team will circle back with daily stand ups.  At the end of the week the team will issue their results in a 1-2 page write up.  They will also walk the entire company through their process and their results as a key component of our monthly all company meeting.  

They will also participate in the nomination of the next team and will send one delegate to answer questions for the next month team as well.
