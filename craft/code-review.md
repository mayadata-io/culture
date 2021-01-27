# Code review

Note: Google's [How to do a code review](https://google.github.io/eng-practices/review/reviewer/) heavily influenced this document.

Code reviews are an essential part of our constant effort to improve quality of our code base. It is essential for keeping technical debt under control. Good code-review is a balancing act. We don't want to allow smelly code, but also going through review should not be a painful process, which will prevent developers from submitting features or improvements.

Key attributes which reviewers are looking for

- proposed change is consistent with the rest of the code-base.
- proposed change is maintainable (or is not making existing code harder to maintain).
- proposed change is improving the overall code health (even if the change itself is not perfect).
- proposed change is addressing product/business need described in the parent ticket.

Only exception when reviewer could approve change which is worsening overall code health is state of **emergency**.

## Principles of code-review

- Technical facts overrule opinions and personal preferences.
- Style is driven by our [coding style guides](coding-style.md). We are striving to keep style consistent across the entire code-base. If something is missing from the style guide, consider proposing a change to it.
- Code design is never purely personal decision. Sometimes there could be several options how to approach a particular problem. Author of the change should be able to demonstrate her decision process and provided reasoning for the solution chosen. Ideally, such thought process is already captured in comments or in the ticket relevant to the change. If proposed solution is equally good to reviewer's alternative, reviewer should accept author's proposal.
- If we don't have explicit rule, reviewer can ask author to keep consistency with the rest of the code base (e.g. don't necessarily use some new language construct, if it obstructs readability of the code given the context).
- Respond to code-review request in a timely manner. If you cannot attend code-review, let the author know and work out if you need to resign as reviewer or review can wait.
- In cases of big code changes, always try to split change into multiple code-reviews. Is your code design correct? Could you leverage feature-flags / configuration more?
- When appropriate, organize **pair code-reviews** where author meets (calls) reviewer and go through the review together. Think about pair-programming applied to reviews. How to realize, that it is time for pair-review:

  - your comments became short novels, instead of couple short sentences;
  - you went through your cup of tea/coffee and you are still not even reached half of the review;
  - you start to question competency of the author;
  - you start to think that the author was working on something totally different in parallel.

### Choosing your code-reviewer

Unfortunately, automation in GitLab is currently very limited. You need to pick your reviewer manually. Phabricator is way better, but we are currently not promoting Differential flow as it is more complicated for a junior developers (also not ideal when you need to collaborate on the top of the code).

Rule of thumb for choosing your reviewer is to **escape your bubble**. Try to ask other people first, then your buddy sitting next you. This helps keeping engagement as well as overall understanding of the code-base. It also helps tremendously with keeping whole code-base consistent.

Also, your current reviewer can always pass the review to somebody else, if she feel appropriate. So don't worry and be curious.

## Key things look for in a code-review

Reviewer should always make sure, that they have thought about the following aspects of the code. Naturally, we expect authors to think about them as well :)

- The code is well designed. (Sensible modularization of the code, appropriate paradigms being used)
- The implementation is actually addressing a need described in the implementation ticket (aka is it doing, what it should be doing?).
- The functionality is good for the user -- if used by programmers, does the API make sense? If UI change, does the change make sense to the users, does it look good?
- Any parallel programming or external services are handled safely (check for race-conditions, deadlocks, missing timeouts).
- The code isn’t more complex than it needs to be.
- The developer isn’t implementing things they might need in the future but don’t know they need now.
- Code is not weakening our security model.
- Code appropriately handles privacy of the users (for example it is not logging unnecessary personal details into application logs).
- Code has appropriate unit tests.
- Tests are well-designed.
- The developer used clear names for everything.
- Comments are clear and useful, and mostly explain why instead of what.
- Code is appropriately documented.
- The code conforms to our style guides.

## Writing code-review description & commit message

When you are author getting ready to submit your fresh change for code-review. Always pay attention to the description of the code-review request. A description is a public record of **what** change is being made and **why** it was made. For writing good description apply the same principles as for writing a good commit message. Therefore we are going to cover them together. For more, read [A Note About Git Commit Messages](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html) from Tim Pope and [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/) from Chris Beams.

We have agreed to follow [Conventional Commits](https://www.conventionalcommits.org/) format. Please, read the specification and go through examples.

Summary of key principles of the good description or commit message:

- Separate subject from body with a blank line.
- Use the imperative mood in the subject line.
- Wrap the body at 72 characters for git commit messages.
- Use the body to explain what and why vs. how.
- Always mention related tickets (no need for full URL, just the ticket id).

### Body is Informative

- Wrap the body at 72 characters for git commit messages.

The rest of the description should be informative. It might include a brief description of the problem that’s being solved, and why this is the best approach. If there are any shortcomings to the approach, they should be mentioned. If relevant, include background information such as bug numbers, benchmark results, and links to design documents.

## Writing code-review comments

As mentioned at our [values](/plow/plow.md), always remember the human-being on the other side of the line. It is really strongly suggested to use pair-reviews for complex or problematic reviews. Always remember to

- expect competency and good intentions;
- be kind;
- comment on the code, never on the person;
- explain your reasoning, ask for explanation of author's reasoning;
- stay constructive -- suggest what should be changed;
- balance between giving explicit directions with just pointing out problems and letting the developer decide.

Also, when you needed substantial time for discussion over some topic, you should consider requesting code-rewrite (to make it more understandable) and/or extend in-code documentation. Also consider updating the implementation ticket with a summary of your findings. Code-review comments are rarely accessed retrospectively. Make a special effort to **capture information**, when doing **pair-review**.

## Emergencies

Sometimes the speed of getting change out to the production outweighs having a polished code. Such change should be a **small** change that: allows a major launch to continue instead of rolling back, fixes a bug significantly affecting users in production, handles a pressing legal issue, closes a major security hole, etc.

In emergencies we really do care about the speed of the entire code review process, not just the speed of response. In this case only, the reviewer should care more about the speed of the review and the correctness of the code (does it actually resolve the emergency?) than anything else. Also (perhaps obviously) such reviews should take priority over all other code reviews, when they come up.

However, after the emergency is resolved you should look over the emergency code-changes again and give them a more thorough review.
