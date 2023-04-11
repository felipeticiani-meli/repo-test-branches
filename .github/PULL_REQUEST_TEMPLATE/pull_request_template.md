<!--
PR INSTRUCTIONS 
Title: make a self-explanatory title describing what the pull request does with few words.
Description: detail with what was changed, why it was changed, and how it was changed.
Reviewers: tag the persons that may revise the PR. One member of from team that owns this project is required.
Assignees: please tag yourself into the assignees box.
Labels: choose the appropriate labels, like, if it's a bug, the label will help the reviewers to give priority to this.
Remove the comments before submitting the PR.
-->

## Description

<!-- Add your description here -->

## Type of change
<!--
Check that are relevant
In case of "Other", you must explain it
-->

- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation's update
- [ ] Database's migration
- [ ] Other

## Author' checklist
### Tests and Security

- [ ] Have I run the unit tests before pushing the changes to github?
- [ ] Have I kept or increased the test coverage?
- [ ] Are any dependencies included in this PR? Did you research if it has vulnerabilities before implementing? It is recommended that you always check a vulnerability database before using a dependency: [Snyk Vulnerability DB](https://security.snyk.io/vuln), [GitHub Advisory Database](https://github.com/advisories), [CVE](https://cve.mitre.org/cve/search_cve_list.html)
- Please, make sure this PR follows these [Custom Cheat Sheets](https://docs.google.com/spreadsheets/d/1Plzl7ZcJqdioGZVYSRNMmFMw18jvopxgJJ5IunuJ3Z4/edit?usp=sharing)
  
### Best Practices

- [ ] Have I changed the documentation to reflect the changes in the code (if needed)?
- [ ] Have I named this PR with a descriptive name?
- [ ] Have I reviewed my commit logs to make sure all commits are atomic and well described? Do I need to squash (or reword) some of them?


### General

- [ ] The code do what the Jira issue is describing
- [ ] Have you checked if this merge with `develop` has conflicts? Please, resolve them before submitting for review.

## Reviewer's checklist

- [ ] All commits are well written, following the [How to write a good commit message](https://chris.beams.io/posts/git-commit/#seven-rules) principles
- [ ] The PR's name is a descriptive one (this name will be shown in changelog)?
- [ ] The tests provided assert the right things and at least the most common use cases
- [ ] This PR follows these [Custom Cheat Sheets](https://docs.google.com/spreadsheets/d/1Plzl7ZcJqdioGZVYSRNMmFMw18jvopxgJJ5IunuJ3Z4/edit?usp=sharing)
 
<!--
Case there's more important things to be done when release, please specify it here
Ex: diagrams, screenshots, external links, instructions...
-->