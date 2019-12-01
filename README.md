# Customized Git Hooks

## commit-msg:

If commit message contains a Jira ticket reference ID-###:
* Add commit message to Jira Issue as a comment
* Add links to Jira issue in git commit message

Tested with Jira REST API v2 for Jira server


`config.sample.json` is an example config file
Edit this file and add
* Jira login user id
* Jira password
* Jira server base url


```json
{
  "user": "YOUR_USER_ID",
  "password": "YOUR_PASSWORD",
  "url": "https://JIRA_SERVER_BASE_URL",
  "base": "/rest/api/2",
  "project": "EN"
}
```


## Install

To install a hook, copy the file and config to `.git/hooks/` directory in your repo.


## Samples

Files ending in `.sample` are the default git hooks that are in any newly created git repo as of 12/1/2019.
