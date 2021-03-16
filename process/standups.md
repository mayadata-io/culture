# Daily Standups

Having a daily stand up is an important part of knowledge sharing. That includes, but it is not limited to:

- what others are doing (to sync or avoid duplication, give opportunity to cooperate);
- express dependencies (e.g. I am waiting for some other event to happen before I can continue with my work);
- highlighting (semi-)important events, new projects, merge request (doesn't replace email for important notifications, but helps with spreading the information);
- highlighting interesting information sources (for example mentioning that interesting meeting happened and where are meeting minutes, mentioning an interesting article or task);
- status update about future plans (are we on track with our long-term goals, is some change in direction coming).

But physical standups (round tables) are frequently non-effective and actually quite hard to follow and don't give opportunity to dig deeper into topics which interests you. Also having a physical standup effectively prevents anybody from a different time-zone to participate.

## How it works?
To address these issues, we have introduced a **written standup**. It works as follows:

- Bot creates an empty document every midnight UTC. File will be created under [standups folder on Google Drive](https://drive.google.com/drive/folders/1HfW3hqDVvhP1kalAiJLAqWTmn6To2DLb). It follows naming schema of `{year}/{month}/{year}-{month}-{day}_standup`. Documents are made as copies of a [template](https://docs.google.com/document/d/1PHKrBLJxgS59x3WILbmUvz1VsvdO1m_xNRveGNvHY-c/edit). So in case, you want to update how standups are going to look like in the future, just edit this document.
- Bot publishes the link to Slack channel [`#engineering-standups`](https://app.slack.com/client/T6PMDQ85N/C01HY3QTJHH). Slack channel makes it really easy to go back couple standups in case you need it.
- Everybody has her/his section in the document.
- Your record in the document should be finalized by the **end of your work day**. In other words -- you are supposed to be capturing what you have *done the same day* or what are you *planning to be doing next day*. It doesn't typically talk about yesterday (in contrast to typical standup).
- On the other hand, when you start working in the morning. Quickly go through the stand up from the **previous day**. That will help you to see what others have done.
- **Always provide context** to allow people to understand the update (links to Jira tasks, Github projects, merge requests or just link what ever you are talking about). Please format links nicely, they are read more often than written.
- If somebody asked a question / requested more details via comment, always consider updating your record in the document (in contrast to just replying to the comment). Any consecutive reader will benefit from updated text.

Please, be reasonable in picking topics to write about. You don't need to cover every single email you have read. Similarly, it would be interesting to make a research around various cuisine across the whole company, but this is not really the place to share what you had for lunch. Basically, always keep on mind, that somebody is going to read it, so pick what is valuable for potential readers.

## Key Benefits of Written Standups

- One can read way faster then listen/speak. So you can cover way more people when reading their notes.
- Having a links to additional resources give opportunity to dig a bit deeper and ask meaningful questions.
- Google Document allows for inline comments which became a great tool for asking additional information asynchronously.
- It is fair for everybody, despite their schedules or time-zones. It turned to be really valuable for us, as we have teams around the globe (Asia, Africa, Europe, Americas). Standup basically follows the sun.
- Allows people who are for any reason missing on a particular standup to catch up easily.
- Produces body of *searchable* and *rich* documents.
- It also helps you to see what you have achieved during the day. And get the sense of accomplishment, which is otherwise challenging to get at knowledge jobs.
- You can use the document as a log-book. Filling it during the day. It removes burden of remembering what you have done at the end of the day. As well as it allows for faster pickup by others.
