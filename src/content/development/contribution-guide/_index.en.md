---
title: "Contributing to the Project"
date: 2022-03-15T10:31:00+02:00
weight: 30
---

This guide outlines the process which developers need to follow when contributing to the Submariner project.
Developers are expected to read and follow the guidelines outlined in this guide and in the other contribution guides,
in order for their contributions to the project to be addressed in a timely manner.

## Project Resources

Submariner uses [GitHub Projects] to manage releases. Read [Tracking progress on your project board] to learn more on how to work with 
projects.

### Backlog Board

[The backlog board] hosts issues or features that are not scheduled for the release currently being developed. While each issue is opened in
its corresponding repository, this board gives an aggregated view of all open issues across all repositories. The board has total of seven
columns. Any issue or epic opened should be assigned to `Backlog` Projects in `Backlog` column. Issues intenteded to be
worked on for the next release are moved to `Next Version Candidate` column. During [pre-planning](#Pre-Planning), issues from the `Next
Version Candidate` column are triaged. Issues or epics properly triaged, with assignees and priority labels addeded, are moved to [current 
release board](#Current Release Board). The next 3 columns are of priority. All unassigned issues are sorted into these three columns
based on the priority discussed in the team meeting. Issues from these columns should be worked upon if the current release work is
finished. Any leftover work from the previous release goes to the `Work in Progess column`. `Close?` column holds any issue/epic that
could probably be closed for various reasons.

### Current Release Board

Current release work is tracked in [the 0.13 board]. THe board has 5 columns. The first one, `Schedule and Epics`, hosts all properly
triaged epics targeted for the current release and schedule for the current release. Triaged issues are under `TO DO` column. When an
issue is being worked on, it is moved to `In Progress` column. When a PR for the issue is pushed, the issue is moved to `In Review`
column. The PR has the corresponding issue linked from the GitHub UI and is not tracked on the board. Once the PR is merged, the issue
is moved to `Done` column.

### Enhancements Repository

All enhancement proposals need to be submitted to the [enhancements repository]. To submit a new enhancement proposal, raise an
[Enhancement Request issue] on the repository.

### Releases Repository

Submariner's release is automated to a great extent. [The release process documentation] explains the details of a release. The release
automation is maintained in the [releases repository]. It also hosts `subctl` binaries for all released versions. 

## Bugs, Tasks and Epics

To be expanded

### Bugs

To be expanded

### Tasks

To be expanded

### Epics

To be expanded

## Release Cycles

The Submariner project follows time based release cycles where each cycle is 16 weeks long.
While blocking bugs may delay the [general availability](#general-availability) release date, new features will not.

Features that were partially implemented in a given release will be considered "experimental" and won't have any support commitment.

Each cycle will result in either a minor version bump or a major version bump in case backwards compatibility can't be maintained.

### Sprints

Sprints are 3 week periods which encapsulate work on the release.
Most sprints focus on active development of the current version, while some focus on additional aspects such as design and stabilization.
Specific sprints and their contents are detailed in the following sections.

Most sprints will end with a milestone pre-release as detailed in the following sections.
This allows the community and project members to verify the project is stable and test any fixes or features that were added during the
sprint.
A formal [test day](#test-days) may be held to facilitate testing of the pre-release.

Each sprint ends on a boundary day which also marks the beginning of the next sprint.
The boundary days occur on a **Monday**.

On the sprint boundary day we will:

* Perform a milestone pre-release (when applicable).
* Have release related meetings, instead of any usually recurring meetings:
  * Grooming (30 minutes):
    * Making sure epics are on track.
    * Reviewing the Definition of Done for each epic.
    * Moving epics back to the Backlog, in case they're de-prioritized.
  * Retrospective (30 minutes):
    * Looking back at the task sizes and assessing if they were correct.
    * General process improvement.
  * Demos (30 minutes):
    * Any enhancements (or parts of) that have been delivered in the sprint.
    * Other interesting changes (e.g. refactors) that aren't part of any epic.
    * In case there's nothing to showcase, this meeting will be skipped.

### Release Timeline

<!-- Source: https://docs.google.com/drawings/d/1wZCogcChCkX2PqoIuTx9I_iOgJuwsYjChVopq1nfqeM -->
![Timeline Diagram](/images/timeline.png)

Each release follows a fixed timeline, with 4 development sprints and one final sprint for stabilization.
The version will be released one week after the last sprint, and the planning work for the next release will begin.

The following sections explain the activities of each sprint.

#### Pre-Planning

To be expanded

#### Feature Design

To be expanded

#### Development Milestones

The milestone sprints are focused on development work for various [tasks](#tasks) and [bugs](#bugs).
Project members will work on any planned tasks and bugs, and will also work on unplanned bugs should they arise.
Any [unplanned work](#unplanned-work) should follow the defined guidelines.

Each sprint will end with a release to allow the community to test new features and fixed bugs.
In total, three milestone sprints are planned:

* Two milestones ending with releases of milestone `m1` and milestone `m2`.
* The last sprint ending with the release of the [release candidate](#release-candidates) `rc0`.

As detailed in the [sprints](#sprints) section, each milestone release will be followed by a test day and the sprint meetings.

#### Release Candidates

At the end of 12 weeks, the project is ready to be released and the pre-release `rc0` is created.
At this point, as detailed in the [release process] documentation, stable branches are created and the project goes into feature freeze
for the release branches.

Two [test days](#test-days) will take place after the release is created, as the project members make sure the release is ready for
[general availability](#general-availability).
Any bugs found during the test days will need to be labeled with the appropriate `testday` label.
The project members will triage the test day bugs and identify any high priority ones that should be addressed before general availability.

If any high priority bugs were identified after `rc0`, a new release `rc1` will be planned to allow for fixing them.
The `rc1` release will be planned at the team's discretion and has no expected date.
If no `rc1` release is planned, the team will proceed with the general availability release.

Starting from `rc1`, the stable branches enter a code freeze mode - only blocker bugs will be eligible for merging.
If a bug is fixed and merged during the code freeze, a new release candidate needs to be prepared and tested.
Releasing `rc2` and beyond will delay the general availability release.

#### General Availability

To be expanded

### Unplanned Work

To be expanded

#### Ongoing Maintenance

To be expanded

#### Exception Process

To be expanded

### Test Days

To be expanded

[release process]: ../release-process
[GitHub Projects]: https://docs.github.com/en/issues/organizing-your-work-with-project-boards
[Tracking progress on your project board]:
(https://docs.github.com/en/issues/organizing-your-work-with-project-boards/tracking-work-with-project-boards)
[The backlog board]: (https://github.com/orgs/submariner-io/projects/15)
[the 0.13 board]: (https://github.com/orgs/submariner-io/projects/20)
[enhancements repository]: (https://github.com/submariner-io/enhancements)
[Enhancement Request issue]: 
(https://github.com/submariner-io/enhancements/issues/new?assignees=&labels=enhancement&template=enhancement.md)
[The release process documentation]: (https://submariner.io/development/release-process/)
[releases repository]: (https://github.com/submariner-io/releases)
