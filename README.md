# init-Newcomer-SG

Aim: Documenting getting up to speed.

## Checklist

Minimum requirements:
- [x] Github account (you should have else you would not be able to view this md file)
- [] G suite account -- your CoverWallet gmail and calendar
- [] Atlassian Confluence account -- you should be able to access [this](https://coverwallet.atlassian.net/wiki/spaces/TECH/overview)
- [] Slack -- ask to be invited to `sgp-developers`, `singapore-tech`, `team-aon-backenders`, `team-aon-frontenders`, `singapore-hr`. Search and join `singapore`, `team-australia`, `tech team`

## Quickstart:

Start with video walk-through: 
recommended to watch the [video](https://drive.google.com/file/d/1dF6qiQW4OEI6gnVGh5m4-b99ZBF-vKEH/view) first as entry point to understand

Overview on architecture:
[Single source of truth](https://coverwallet.atlassian.net/wiki/spaces/AON/pages/2324529185/Australia+technical+Overview)

For any unfamiliar terms:
refer to this [WIP glossary](https://coverwallet.atlassian.net/wiki/spaces/AON/pages/2686779454/Basic+AUS+glossary)

[All other video walkthroughs](https://drive.google.com/drive/folders/1RPiGurBoze4UPhXh7BNZTOn5gtKH713Y)

---

BE quickstart locally requirements:
1. Have ruby 2.5.1 installed with RVM
2. MongoDB (can use docker image if you do not want to persist data)

Or to use docker, refer to [readme here] (https://github.com/coverwallet/aon-quotes)

## Development cycle

Summary (For AUS project):
- get your task from [jira](https://coverwallet.atlassian.net/secure/RapidBoard.jspa?rapidView=120&projectKey=AONC#). open a branch from master
- do your job, write a lot of tests for it. (even better if you do TDD)
- push the branch and open a PR (and ask someone to review)
- apply the feedback you receive if any and once the PR has been approved merge it into `beta` branch. push it
- `beta` is the branch where developers and sometimes QA checks that what we have done works
- once you are satisfied with the result merge your branch in `uat` branch and push it. Sometimes this step is not allowed, normally when carriers are testing something and they need the UAT environment as much stable as possible
- once QA (so Hanna) approves your work you can rebase your branch with master and click the green button to merge it
- last step go to the #deploys channel and summon the deploy bot: candi to launch the deploy (to check how every push you do goes you can look in our CI/CD tool, [here](https://app.circleci.com/pipelines/github/coverwallet/aon-quotes))


### People to reach out to via slack:
