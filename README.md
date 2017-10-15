# Maintenance Guidelines for textlint-rule organization

This guideline is for existing or new members of textlint-rule organization.

This document show guide of procedures for adding packages, adding new member.

## Principles

- To avoid human bottlenecks
- To trust people to do the right thing until proven otherwise

In order to minimize human bottlenecks, all members should be fully empowered to do everything that might be necessary to handle administration of the project.

For some actions, it might be good to discuss with other members and the community about the best course of action.
For other decisions, it might be better to take individual initiative.

Instances of untrusted behavior may be reported by contacting the project team at azuciao+textlint@gmail.com. 
Untrusted behavior is defined in [Code of Conduct][].

All complaints will be reviewed and investigated and will result in a response that is deemed necessary and appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident.

## For maintainer

Maintainer can add new members to the project liberally.

If you identify someone who is interested in the project, seems trustworthy, and agrees to the [Code of Conduct][], you can follow the steps below.

### GitHub

1. Visit <https://github.com/orgs/textlint-rule/people>
2. Click **Invite member**
3. Type the username or email address of the person you want to invite and click Enter
4. Set the radio button to "**Owner**"
5. Send Invitation

For more infromation, see [Inviting users to join your organization - User Documentation](https://help.github.com/articles/inviting-users-to-join-your-organization/)

### npm

1. Visit <https://www.npmjs.com/org/textlint-rule/members>
2. Type the username or email address of the person you want to invite
3. Set the radio button to "**Owner**"
4. Click **add member**

For more infromation, see [Managing Members · npm Orgs Documentation](https://www.npmjs.com/docs/orgs/managing-members.html)

## For new member

To add a package to the organization, you can follow the steps below.

### GitHub

Transfer your repository's ownership to the organization.

1. Visit <https://github.com/$USER/$PROJECT/settings> (Your repository setting page)
2. Click **Transfer** on Danger Zone
3. Type textlint-rule in the field labeled "New owner's GitHub username or organization name"
4. Click "I understand, transfer this repository" button
5. After transfer, modify meta-data in pacakge.json, README.md, and Re-Enable CI etc...
  - Utils: [transfer-github-owner](https://github.com/azu/transfer-github-owner "transfer-github-owner")

For more infromation, see [About repository transfers - User Documentation](https://help.github.com/articles/about-repository-transfers/)

### npm

Run this command, replacing `$PKGNAME` with the name of the package on npm:

```shell-session
npm access grant read-write textlint-rule:developers $PKGNAME
```

OR

1. Visit <https://www.npmjs.com/org/textlint-rule/team/developers/add-package>
2. Select your package name in "Populate from personal packages"
3. Click **make it so** button

For more infromation, see [Managing Package Access · npm Orgs Documentation](https://www.npmjs.com/docs/orgs/managing-package-access.html)

## Attribution

This Guideline is adapted from the [Maintenance Guidelines for Organization](https://maintenance-guidelines-for-organization.github.io/).

This Guideline is available under Creative Commons Attribution 4.0 International Public License([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).

[Code of Conduct]: ./CODE_OF_CONDUCT.md
