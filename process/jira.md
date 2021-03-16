# Jira Hygiene

As almost anything even Jira requires regular maintenance to address:

-   Incomplete/unclear tickets
-   Stale/outdated tickets
-   Forgotten/unpopular tickets
-   Usefulness of Jira content as a whole

Why? Even though it might not look like it at first glance, Jira is a tool to *communicate with* people in an open, transparent and remote-friendly manner and facilitate *reaching our goals*. This text tries to apply our [PLOW](https://culture.mayadata.io/plow/plow.html) to working with Jira. To keep various Jira projects open and welcoming. To allow us to cooperate effectively and win - personally and professionally and deliver the value that is useful to the company and open-source community in a repeatable and dependable manner.

## Two loops

For Jira to be an effective communication tool, information must flow freely while being taken care of at every stage.

### Loop one \-- Initial Triage

Person responsible for maintenance should regularly \-- **at least daily** \-- check new tickets flowing into the project (status *open*). In case of projects that can receive time sensitive tasks (e.g. operations/SRE, customer support) it is recommended to set up a notification channel for new tickets (if you like email - see [PLOW-22](https://mayadata.atlassian.net/browse/PLOW-22);
there's a possibility to send new tickets to slack channel but consider that shared responsibility often doesn't work and unnecessary interrupts and notifications are especially harmful to deep complex work we do here, so it is recommended to point this integration to a special channel for this purpose. Especially avoid channels with more than few involved members).

It is required to take care of every new ticket, it does not mean that every ticket will be worked on when received. Probably incomplete list of what to do with new tasks:

-   Ticket is **clear, understandable** and **actionable**, contains **why**, **what** and any particularities required. Also has all required metadata. It is aligned with team priorities, [OKRs](https://culture.mayadata.io/process/okr.html) and company's strategy. Such tickets should be *accepted for prioritization*. In case of urgent tickets these must skip prioritization and must be taken care of immediately with clearly agreed ownership.

-   If a ticket does not fit any or all criteria written above it must be fixed. Possibly by:
    -   Adding additional information if known to a particular project maintainer
    -   Making required decisions if applicable.
    -   Reaching out to the author (ticket assignment works well) to provide missing pieces or explanation, alignment of priorities - *consider* having shorter discussions in slack as when ticket description is fixed and/or augmented, comments *might* become perplexing or superfluous to further work with the ticket and make communication harder not easier. If you need longer discussion, a design document/meeting or similar tool should probably be used. It is the project maintainer's responsibility to make sure this happens.
    -   Closing the ticket with a good description of why you did that (duplicate tickets are an obvious example).
    -   Moving ticket to a different project if appropriate.

### Loop two \-- Health Check

Even if every new ticket is catered for projects always tend to accumulate a bit of dust. For that reason regular review of **all project's tickets** needs to be done. It is recommended doing that on a **weekly** basis. Ideally most of the work described here is done by the ticket owner but loop two *guarantees* that it happens even if for any reason the owner hasn't or couldn't.

This would mainly consist of:

-   Going through **all tickets one by one** (from experience, after few iterations it can be done in about 30 minutes for a 500 ticket board of a sizeable team)
-   Validating each ticket still makes sense and is correctly prioritized as in agile development priorities might shift wildly. In case of failure to pass this test ticket should be deprioritized or even closed with a clear comment why. Consider commenting even when deprioritizing to keep - potentially unknown - colleagues and stakeholders in the loop and able to react.
-   Making sure unpopular/maintenance/forgotten tickets are taken care of eventually.
-   Validating all tickets have proper status:
    -   Are in-progress tickets progressing? (communicating by putting ticket back from in progress to previous states is valid fix)
    -   Are blocked tickets still blocked?
    -   Are PRs being done in a timely manner?
-   Is someone struggling with a ticket without a reaction?
-   Validating miscellaneous conditions like are in-progress tickets assigned, all stakeholders are kept in the loop, etc.
-   Ticket updates/comments are also clear and understandable. Questions are answered.
-   Giving the team a good pat on the back for its work.

## Responsibilities and Perks

Main responsibility to make this happen is on [Lead Engineer](https://culture.mayadata.io/job-roles/lead-engineer.html) (put your [project manager](https://culture.mayadata.io/job-roles/lead-engineer.html#project-management)'s hat on), however she/he might choose to delegate or rotate responsibilities in the team. Some of the responsibilities might also be automated. Until they are, they however must be done manually. [Lead Engineer](https://culture.mayadata.io/job-roles/lead-engineer.html) should motivate the team to keep its Jira as clean as possible by default.

It is recommended that *loop two* be done by [Lead Engineer](https://culture.mayadata.io/job-roles/lead-engineer.html) herself/himself before the team\'s regular grooming/prioritization sessions. It will have additional value of coming to grooming/prioritization meetings prepared with refreshed knowledge of tasks at hand as [Lead Engineer](https://culture.mayadata.io/job-roles/lead-engineer.html) often has to explain work at hand in terms of why and how it connects to other tasks in near term, other projects and motivate team members to do the work by conveying its purpose and meaning in a broader context. Moreover regular maintenance of workboard brings intuitive understanding of team's current priorities and short/mid-term plans which, from experience, is quite useful for leadership role and helps with many responsibilities [Lead Engineer](https://culture.mayadata.io/job-roles/lead-engineer.html) has as reporting progress outside the team (if at all needed with clean project), answering and aligning team members about priorities, avoiding work duplication and in general keeping the team "well oiled" and working at its best performance. And it feels really good.
