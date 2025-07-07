# Community membership

This docs different ways to get involved and level up within the project. You can see different roles within the project in the contributor roles.

**Note:** This document is a work in progress

This doc outlines the various responsibilities of contributor roles in HAMi.

| Role       | Responsibilities                                              | Requirements                                                       | Defined by                   |
|------------|---------------------------------------------------------------|--------------------------------------------------------------------|------------------------------|
| Member     | Active contributor in the community                           | Sponsored by 2 reviewers and multiple contributions to the project | HAMi GitHub org member    |
| Reviewer   | Review contributions from other members                       | History of review and authorship in a subproject                   | [OWNERS] file reviewer entry |
| Approver   | Contributions acceptance approval                             | Highly experienced active reviewer and contributor to a subproject | [OWNERS] file approver entry |
| Maintainer | Demonstrated responsibility and excellent technical judgement | Demonstrated responsibility and excellent technical judgement      | [Maintainers] file entry     |

**Note :** It is mandatory for all HAMi community members to follow HAMi [Code of Conduct](./CODE-OF-CONDUCT.md).

## New contributors

[New contributors] should be welcomed to the community by existing members,
helped with PR workflow, and directed to relevant documentation and
communication channels.

## Member

Members are continuously active contributors in the community. They can have
issues and PRs assigned to them, participate in SIGs through GitHub teams.
Members are expected to remain active contributors to the community.

**Defined by:** Member of the HAMi GitHub organization

### Requirements

- Sponsor from 2 approvers
- Enabled [two-factor authentication] on their GitHub account
- Actively contributed to the community. Contributions may include, but are not limited to:
  - 5 accepted PRs be **merged**.
  - Reviewed 5 PRs,
  - Resolved and closed 3 Issues,
  - Participate in HAMi community meetings
  - Participating in community discussions on slack/mailing/meetings list
  - Become responsible for a key project management area or some equivalent combination or contribution
- Must have been contributing for at least 3 months
- Must be actively contributing to at least one project area
- Must have two sponsors who are also Organization Members, at least one of whom does not work for the same employer
- **[Open an issue][membership request] against the HAMi/community repo**
 - Ensure your sponsors are @mentioned on the issue
 - Complete every item on the issue checklist
 - Make sure that the list of contributions included is representative of your work on the project.
- Have your sponsoring reviewers reply confirmation of sponsorship: `+1`
- Once your sponsors have responded, your request will be handled by the `HAMi GitHub Admin team`.

### Responsibilities and privileges

- Member of the HAMi GitHub organization
- Issues and PRs can request their review
- Participate in assigned issues and PRs
- Welcome new contributors
- Guide new contributors to relevant docs/files
- Help/Motivate new members in contributing to HAMi

## Reviewer

Reviewers are able to review code for quality and correctness on some part of a
subproject. They are knowledgeable about both the codebase and software
engineering principles.

**Defined by:** *reviewers* entry in an OWNERS file in a repo owned by the
HAMi project.

### Requirements

The following apply to the part of codebase for which one would be a reviewer in
the [OWNERS] file (for repos using the bot).

- member for at least 3 months
- Primary reviewer for at least 10 PRs to the codebase
- Reviewed or merged at least 20 substantial PRs to the codebase
- Knowledgeable about the codebase
- Sponsor from 2 maintainers
  - With no objections from other approvers
  - Done through PR to update the OWNERS file
- May either self-nominate, be nominated by an approver in this subproject.
- Make an agenda in weekly meeting with no objections from other reviewers, approvers, and maintainers

The following apply for a sub-project reviewer, for example(HAMi-webui, volcano-vgpu-device-plugin, etc..)

- Satisfy Either
  - Initial contributer of the sub-project
- OR 
  - Primary reviewer for at least 5 PRs to the codebase
  - Reviewed or merged at least 5 substantial PRs to the codebase
- Knowledgeable about the codebase
- Sponsor from 1 maintainer
  - With no objections from other approvers
  - Done through PR to update the OWNERS file
- May either self-nominate, be nominated by an approver or maintainer in this subproject.
- Make an agenda in weekly meeting with no objections from other reviewers, approvers, and maintainers

### Responsibilities and privileges

The following apply to the part of codebase for which one would be a reviewer in
an [OWNERS] file (for repos using the bot).

- Code reviewer status may be a precondition to accepting large code contributions
- Responsible for project quality control
  - Focus on code quality and correctness, including testing and factoring
  - May also review for more holistic issues, but not a requirement
- Expected to be responsive to review requests
- Assigned PRs to review related to subproject of expertise
- Assigned test bugs related to subproject of expertise
- May get a badge on PR and issue comments

## Approver

Code approvers are able to both review and approve code contributions.  While
code review is focused on code quality and correctness, approval is focused on
holistic acceptance of a contribution including: backwards / forwards
compatibility, adhering to API and flag conventions, subtle performance and
correctness issues, interactions with other parts of the system, etc.

**Defined by:** *approvers* entry in an OWNERS file in a repo owned by the
HAMi project.

### Requirements

The following apply to the part of codebase for which one would be an approver
in an [OWNERS] file (for repos using the bot).

- Reviewer of the codebase for at least 3 months
- Primary reviewer for at least 10 substantial PRs to the codebase
- Reviewed or merged at least 30 PRs to the codebase
- Sponsor from 2 maintainers
  - With no objections from other subproject owners
  - Done through PR to update the OWNERS file
- Nominated by a maintainer and pass super-majority(two-thirds/ 66.66%) vote.

The following apply for a sub-project approver, for example(HAMi-webui, volcano-vgpu-device-plugin, etc..)

- Satisfy Either
  - Initial contributer of the sub-project 
- OR
  - Reviewer of the codebase for at least 3 months
  - Primary reviewer for at least 10 PRs to the codebase
  - Reviewed or merged at least 10 substantial PRs to the codebase
- Knowledgeable about the codebase
- Sponsor from 1 maintainer
  - With no objections from other approvers
  - Done through PR to update the OWNERS file
- May either self-nominate, be nominated by an approver or maintainer in this subproject.
- Make an agenda in weekly meeting with no objections from other reviewers, approvers, and maintainers

### Responsibilities and privileges

The following apply to the part of codebase for which one would be an approver
in an [OWNERS] file (for repos using the bot).

- Approver status may be a precondition to accepting large code contributions
- Demonstrate sound technical judgement
- Responsible for project quality control
  - Focus on holistic acceptance of contribution such as dependencies with other features, backwards / forwards
    compatibility, API and flag definitions, etc
- Expected to be responsive to review requests
- Mentor contributors and reviewers
- May approve code contributions for acceptance

## Maintainer

Description: Maintainers are very established contributors who are responsible for the entire project. As such, they have the ability to approve PRs against any area of the project, and are expected to participate in making decisions about the strategy and priorities of the project.

The current list of maintainers can be found in the [MAINTAINERS](https://github.com/Project-HAMi/HAMi/blob/master/MAINTAINERS.md).

### Requirements

- Deep understanding of the technical goals and direction of the project.
- Deep understanding of the technical domain (specifically the language) of the project.
- Sustained contributions to design and direction by doing all of:
  - Authoring and reviewing proposals
  - Initiating, contributing and resolving discussions (e.g. emails, GitHub issues, meetings)
  - Identifying subtle or complex issues in designs and implementation PRs
- Approver for at least 3 months
- Nominated by a maintainer and pass super-majority(two-thirds/ 66.66%) vote.

### Responsibilities and privileges

- Maintaining the project: responsible for ensuring that the project remains stable, 
  secure, and up-to-date, including fixing bugs, addressing security vulnerabilities 
  and releasing new versions of the project as needed.
- Managing contributions: responsible for managing contributions to the project, 
  including code/non-code contributions, bug reports and feature requests.
- Communicating with the community: responsible for communicating with the project's
  community, including users, developers, and other contributors. This may involve
  responding to questions, addressing concerns, and providing updates on the project's
  status.
- Setting project goals and priorities: responsible for setting the project's goal
  and priorities, and for ensuring that the project remains aligned with these goals
  over time.
- Ensuring project sustainability: responsible for ensuring that the project remains
  sustainable over the long-term, including managing dependencies, ensuring compatibility
  with other projects, and planning for the future of the project.

## Inactivity

It is important for contributors to be and stay active to set an example and show commitment to the project. Inactivity is harmful to the project as it may lead to unexpected delays, contributor attrition, and a lost of trust in the project.

* Inactivity is measured by:
  * Periods of no contributions for longer than 12 months
  * Periods of no communication for longer than 12 months
* Consequences of being inactive include:
  * Involuntary removal or demotion
  * Being asked to move to Emeritus status

## Involuntary Removal or Demotion

Involuntary removal/demotion of a contributor happens when responsibilities and requirements aren't being met. This may include repeated patterns of inactivity, extended period of inactivity, a period of failing to meet the requirements of your role, and/or a violation of the Code of Conduct. This process is important because it protects the community and its deliverables while also opens up opportunities for new contributors to step in.

Involuntary removal or demotion is handled through a vote by a majority of the current Maintainers.

[two-factor authentication]: https://help.github.com/articles/about-two-factor-authentication
[OWNERS]: https://github.com/Project-HAMi/HAMi/blob/master/OWNERS
[New contributors]: /contributing.md
[Maintainers]: https://github.com/Project-HAMi/HAMi/blob/master/MAINTAINERS.md
