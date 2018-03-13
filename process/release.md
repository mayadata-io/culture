# Product Release
- The goal is to make a release every month or earlier with features that are required by the users.  For MayaOnline we believe in releasing at least daily.
- We are going to be driven mainly by the data on the quality metrics not by management push (such as, let us release today otherwise we are going to suffer a deviation from the planned milestone) 
- Release Managers (Gates and gate managers)  are clearly defined and system suffers a dearly when quality is not matching as measured by an automated test system.
- There are going to be situations where it makes business sense to gain more market visibility that drives the releases, in such cases, the features delivered are tagged appropriately - as alpha, beta and stable based on the metrics.



MayaOnline Release process

Owner/SRE: Mayur

Key stakeholders:
Product Management - Ajesh
Development - Vishnu Attur
Product Quality - Giridhar Prasad

Release schedule:

Once in a day (Weekdays). 5PM IST
Go/Nogo meeting((over the slack) : 4PM IST 


Every component/module  would be packaged as a  helm chart  versioned in the format <module>-<major_version_#>-<minor_version_#>-<release_version_#>-<commit_sha>*

Every branch runs through the various stages in our CI/CD pipeline :
Stage 1 : Clone the source repo for the branch to be built
Stage 2:  Build the code and package it as a docker image
Stage 3: Run the unit test suite, gather test coverage and publish it
Stage 3: Run the static analysis of vulnerabilities in application containers
Stage 4: Push the docker image to docker hub
Stage 5: Create a helm chart for the module and publish it.
Stage 6: Deploy the helm chart and send a notification to the #production in slack.
Stage 7: Run the integration test for the entire application and publish the report.

Staging branch of every module gets deployed to staging namespace.
Similarly, master branch gets deployed to production cluster(namespace)



For deployments to the production environment, we follow a release process to make sure we release the stable artefacts. Deployments to master require a PR to be raised from staging to master that results in a PR-merge branch(this happens in jenkins and needs to be tested) that needs to go through all the 7 stages described above in a pre-prod cluster(namespace). This PR may consist of “n” number of PRs merged into the staging from their respective feature/bugfix branches and needs to be reviewed and approved by module lead, SRE(to make), QA and the management(product manager, etc.,)

Responsibilities of various teams during a production deployment include but is not limited to :

Module lead:
Capture the unit test cases added for this release
PRs with appropriate description that have been merged into staging. Squash commits generally carry all relevant data. Also make sure that the PR had been assigned a zenhub issue.
Inform the SRE team on whether it was a major/minor release as mentioned up. SRE can then bump up the helm versions accordingly.

SRE 
Create a new release branch conforming to the nomenclature and annotated tags.
Work with the developers to raise a pull request against the master and run the CI suite.
Makes sure only approved features and bug fixes make it to production.
Checklist has been duly followed by the module leads.
Any special provisions needed for deployment?  Gather the information from the module leads and draft it in DR/notes.
Release notes are available for publishing to the customer.
Disaster recovery plan has been drafted and the on-call group has been constituted to monitor and take any actions on MO if needed.
Vote as GO/NOGO for the release to be deployed and let the team know as to why they think so. 

QA 
Make sure that automation QA suite has run against the latest build in pre-prod
Dedicate a QA team member for post deployment quick sanity checks and let the stakeholders know.
Vote/Veto for the release to be deployed on the production supporting it with their arguments in favor or against it,
Perform a load testing on the cluster and present the report to the team

All the the discussion pertaining to the production deployment happens in the #production channel. Our goal is to automate our recordings and actions via slack being our primary chatops tool for deployment and publishing reports. Initially, we may be running a few manual steps but once such action items are identified, SRE will add them as an action item for their forthcoming sprints.

Disaster recovery and rollbacks:
Ours would be an immutable infrastructure i.e., we would deploy only a blessed image to the production i.e., no changes to the server or our deployments via manual 

A blessed release is one that was built when staging branch is merged into master, runs all basic sanity checks, demonstrates a confident test coverage in CI and has been approved by all stakeholders - module lead, QA  and SRE. There could be cases of dependent deployments wherein one module would be dependent on the other and also the chronological order of deployment may be of significance.We do not make the incremental changes to the infrastructure but instead a new one would be spawned and the previous image is still available for rollback of the environment itself to a good known state. 

Note:
* Refer https://semver.org/
