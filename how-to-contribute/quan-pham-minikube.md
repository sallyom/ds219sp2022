Finding issues to work on
- "good first issue": issues where there is a clear path to resolution
- "help wanted": issues where a need has been identified but not resources to work on them
- "priority/important-soon" or "priority/important-longterm": high impact issues that need to be addressed in the next couple of releases
- Ask on #minikube Slack if unsure
- Once you've discovered an issue to work on:
	+ Add a comment mentioning that you plan to work on the issue
	+ Send a PR out that mentions the issue
	+ Comment on the issue with /assign to assign it to yourself

clone minikube (after forking):
git clone git@github.com:kubernetes/minikube.git
cd minikube
git remote rename origin upstream
git remote set-url --push upstream NO_PUSH
git remote add origin git@github.com:<YOUR_GITHUB_USERNAME>/minikube.git

Contribute a patch:
1. Submit an issue describing your proposed change
2. A reviewer will respond to your issue promptly
3. If your proposed change is accepted, and you haven't already done so, sign the Contributor License Agreement (CLA)
4. Fork the minikube repository, develop and test your code changes.
	- Before test, you may need to install some prerequisites
5. Submit a pull request

