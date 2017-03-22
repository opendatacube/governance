# New Subproject Process

The Open Data Cube is organized as a set of Subprojects that are each a GitHub repository with a
development team that follows the Open Data Cube governance, license and contribution model. Officially supported and maintained Subprojects are hosted on the [Open Data Cube](https://github.com/opendatacube) GitHub orgnization. This document describes the process by which new Subprojects are created in or moved to the Open Data Cube organization.

There are two ways that new Subprojects are created:

1. Direct Subproject creation.
2. Incorporation of an existing external Subproject.


## Criteria for official Subprojects

The following criteria will be used in evaluating Subprojects for incorporation into the official
Open Data Cube organization. These apply to any Subproject, regardless of who is developing the
Subproject. Subprojects should:

* Have an active developer community that offers a sustainable model for future development.
* Use solid software engineering with documentation and tests hosted with appropriate
  technologies ([Read The Docs](https://readthedocs.org/) and [Travis](https://travis-ci.org/)
  are examples of technologies that can be used).
* Demonstrate continued growth and development.
* Integrate well with other official Subprojects where appropriate.
* Be developed according to the Open Data Cube [governance and contribution model](https://github.com/opendatacube/governance).
* Have a well-defined scope.
* Be packaged using appropriate technologies such as pip, conda, npm, bower, docker, etc.

As a general guideline, we support improving existing Subprojects over incorporating competing Subprojects in the Project.

The most important question in evaluating Subprojects for incorporation as official Subprojects
is this: is there broad agreement in the community and Steering Council that we are going to
develop and maintain the Subproject in an official capacity?

The two paths for official Subproject creation are now detailed.


## Direct Subproject creation

In some cases, Steering Council members can immediately create new official Subprojects in the main
Open Data Cube organization. This option will be used when the new Subproject is clearly part of the
existing scope, activities and development of the Open Data Cube. The process for direct Subproject
creation is minimal and informal: Steering Council members should be in consensus about the
Subproject's creation and notify the main Open Data Cube list of its creation.


## Incorporation of an existing external Subproject

In other cases, Subprojects proposed for incorporation will have existed and been developed as
open-source software for some time outside the official Open Data Cube organization. This section describes
the incorporation process for these existing external Subprojects. This process applies to
Subprojects that have incubated under the `opendatacube-incubator` GitHub organization (see below),
Subprojects developed under other GitHub organizations or Subprojects developed as open-source
software in other public venues.

When a Subproject is incorporated, it becomes an officialy supported and maintained part
of Project Open Data Cube and is moved to the [Open Data Cube](https://github.com/opendatacube) GitHub organization.


### Proposal for incorporation

For an existing external Subproject to be incorporated into the main Open Data Cube organization, the
following proposal process will be used:

1. The Subproject team should submit a pull request against the
   [opendatacube/enhancement-proposals](https://github.com/opendatacube/enhancement-proposals) repository
   with an enhancement proposal for including the Subproject in the main Open Data Cube organization.
   The enhancement proposal should describe how the Subproject meets each of the above criteria.
2. The proposal for incorporation will be discussed by the community using that pull request.
3. A recommendation will be made by the consensus of the Steering Council (SC).

**Timeline:** the SC should make every effort to reach a decision promptly. If
there is active discussion and feedback about the proposal, that should be
allowed to proceed and voices be heard.  But to avoid unnecessary delays waiting for everyone to vote, the following guideline should be used:

* upon proposal, allow a week for potential objections (explicit agreement
  welcome, of course). If no objections, treat silence as agreement.

* if a month goes by and there's continued, active disagreement, that should be
  treated as a strong signal that the project isn't ready to graduate.

The possible recommendations of the Steering Council will be:

* Integration into an existing official Suproject.
* Incorporation as a new official Subproject.
* Further internal or external incubation (see below) with recommendations on steps the team can
  take to prepare for future incorporation.
* Rejection. This option will be used if the Steering Council thinks the proposed Subproject is not
  progressing or will never be appropriate for incorporation. If a rejected Subproject has been
  incubating under the [opendatacube-incubator](https://github.com/opendatacube-incubator) GitHub
  organization, its repository will be removed from that organization after a transition period.

### Incorporation

When an existing external Subproject is incorporated as a new official Subproject, the following
steps will be taken:

1. The repository will be transfered over to the main Open Data Cube GitHub organization.
2. A GitHub team will be created for the Subproject, with the Subproject team having
   read/write permissions on the Subproject repository.
3. The team will send an email to the main Open Data Cube list with an announcement about the new
   Subproject.
4. The standard [Open Data Cube LICENSE](https://raw.githubusercontent.com/opendatacube/governance/master/projectlicense.md) file that
   is maintained in this governance repository will be added to the repository.
5. Copyright notices in individual files should be updated to the standard form described
   in our [Open Data Cube License](https://raw.githubusercontent.com/opendatacube/governance/master/projectlicense.md).


## Incubation of Subprojects

Incubation refers to the process of a Subproject initially being developed outside the official
Open Data Cube organization. Incubation is recommended for new Subprojects with the following
characteristics:

* Significant unanswered technical questions or uncertainties that require exploration.
* Entirely new directions, scopes or ideas that haven't been vetted with the community.
* Significant, already existing code bases where it is not clear how the Subproject will
  integrate with the rest of Open Data Cube.

Incubation also allows the broader community to easily distinguish between stable, officially
supported and maintained Subprojects in the main GitHub organization and new efforts that are
emerging and being developed for future inclusion.

If there are questions about whether incubation is appropriate for a given Subproject, interested
parties should simply start a discussion on the main Open Data Cube list to get community and Steering
Council feedback.


### Incubation in the [opendatacube-incubator](https://github.com/opendatacube-incubator) organization

If a Subproject team knows from the start that it would eventually like its Subproject to be part
of the official Open Data Cube organization, it can be incubated in the
[opendatacube-incubator](https://github.com/opendatacube-incubator) organization.

The goals of the incubation in the [opendatacube-incubator](https://github.com/opendatacube-incubator) organization are as follows:

* Contributors can quickly and easily get their code exposed to the Open Data Cube community while
  complying with individual and organizational contribution restrictions.
* Contributors can work with the community and Steering Council and gather feedback early and often
  that will help them develop and refine a clear and concise integration proposal.
* Allow the community to distinguish between officially supported Subprojects and experimental
  Subprojects pursued by members of the community.


#### Repository management policy for incubator projects

Projects may from time to time want to create new repositories to explore
various ideas.  The basic policy for this is the following:

* If the project is named `foo`, it can create new repositories named `foo-X`
  without asking for further authorization.  The project can decide whether to
  announce the repo on the broader Open Data Cube channels or not if it thinks there
  is sufficient interest (obviously these repos are still public and open to
  participation by all).

* If the project would like to create a repo named `bar` (a top-level name that
  someone else might potentially be interested in), it should post to the main
  Open Data Cube list.  The proposal will be discussed with the assumption that,
  unless someone raises a serious objection, these requests will be approved as
  propmptly as possible.

### Proposal for incubation

A Subproject team can initiate the [opendatacube-incubator](https://github.com/opendatacube-incubator)
incubation process by submitting a proposal for incubation. This process is designed to be
lightweight and quick:

1. The proposers must fill out an incubation application by sumitting a pull request to the
   [opendatacube-incubator/proposals](https://github.com/opendatacube-incubator/proposals) repository.
2. Proposers must announce their intent to the community with a post to the main Open Data Cube
   mailing list.
3. The proposed Subproject must have an Advocate who is an active Steering Council member. The role
   of the Advocate is to introduce the Subproject team to the Open Data Cube community and help them through
   incubation processes. While the Advocate may be involved in the actual development and design
   of the Subproject, that is not required.
4. The proposal for incubation will be discussed by the community and approved or rejected by
   the consensus of the Steering Council.
5. If approved, the proposal pull request will be merged, if rejected, it will be closed.

### Incubation period

Once a Subproject is approved for incubation in the
[opendatacube-incubator](https://github.com/opendatacube-incubator) organization, the following steps will be
taken:

1. A GitHub repository will be created under the Open Data Cube-incubator organization
2. A GitHub team will be created with read/write access to the repository, including the
   Advocate.
4. The standard Open Data Cube [LICENSE](https://raw.githubusercontent.com/opendatacube/governance/master/projectlicense.md) file that
   is maintained in this governance repository will be added to the new repository.
4. A member of the Steering Council will announce the newly incubated Subproject on the
   main Open Data Cube list.

The goal of the incubation period is to demonstrate that the Subproject is going to develop an
active developer and user community. There is no particular length of time required for incubation,
but it is expected that most Subprojects will be in incubation for at least six months to one year.


## External incubation

Incubation outside the [opendatacube-incubator](https://github.com/opendatacube-incubator) organization is also
possible. In this case, there is no formal process. Any individual or organization can simply create
a new project on their own personal GitHub (or other VCS) repository and develop it as they see fit.
If such an externally created and incubated Subproject wants to become part of the official Open Data Cube
organization, the criteria listed at the top of this document must be satisfied and the same
incorporation process must be followed.
