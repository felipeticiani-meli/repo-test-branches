---
name: Feature release
about: New feature or request
title: ''
labels: 'enhancement'
assignees: ''

---
# Release Flow Checklist

<!--- This Issue should be named as `dd/MM/yyyy - Release`, if there is already an issue with this name, dont worry! Just add `2` to the end. We'll rename it after the version number is defined. --->

This is the step-by-step checklist to create a new release of IPA Api and deploy it, you just need to follow the steps and everything will be right.

Detailed information about steps can be found in the [Release Process Manual](https://github.com/mercadolibre/fury_shipping-tech-docs/blob/master/docs/guide/framework/doc/guides/release/release_guide_pt.md).

## Steps

<!--- This is the default steps to follow, add any step that you think is necessary for this release --->

- [ ] Make sure everything is merged to `develop`
- [ ] Update your local repository
- [ ] Check what kind of changes were made and define next version number
- [ ] Rename release issue to the following pattern: `dd/MM/yyyy - Release <version>`
- [ ] Create release branch following the pattern: `release/<version>`
- [ ] Generate changelog using the command: `make changelog version=<version>`
- [ ] Commit the updated CHANGELOG.md file using the command: `git add CHANGELOG.md && git commit -m "Update changelog to version <version>"`
- [ ] Push release branch
- [ ] Create release pull request
- [ ] Link this issue to release's pull request
- [ ] Update configurations in test scopes (and template if needed)
- [ ] Deploy configurations in test scopes (if needed)
- [ ] Deploy release candidate generated to test scopes
- [ ] Check metrics to ensure everything is ok
- [ ] Merge release pull request to master
- [ ] Run database migrations (if needed)
- [ ] Update configurations in all productive scopes (if needed)
- [ ] Deploy configurations in all productive scopes (if needed)
- [ ] Deploy generated final version to all productive scopes
- [ ] Post to Slack Channel that the deploy was done with success [#help-ipa](https://meli.slack.com/channels/help-ipa)
- [ ] Post to Workplace Group that the deploy was done with success [IPA](https://meli.workplace.com/groups/892585208081296)
- [ ] Merge backport pull request to develop

*Good Job! :)*