---
title: "Contributing to the Project"
date: 2022-03-15T10:31:00+02:00
weight: 30
---

This guide outlines the process which developers need to follow when contributing to the Submariner project.
Developers are expected to read and follow the guidelines outlined in this guide and in the other contribution guides,
in order for their contributions to the project to be addressed in a timely manner.

## Project Resources

To be expanded

### Backlog Board

To be expanded

### Current Release Board

To be expanded

### Enhancements Repository

To be expanded

### Releases Repository

To be expanded

## Bugs, Tasks and Epics

To be expanded

### Bugs

To be expanded

### Tasks

To be expanded

### Epics

To be expanded

## Release Cycles

To be expanded

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

To be expanded

#### Release Candidates

To be expanded

#### General Availability

Once a release candidate is deemed stable and has no blocker bugs it will be released for general availability.
Prior to releasing, the release manager will verify that there have been no changes on the stable branches since the last release
candidate.
This ensures that the release version is as stable as possible, and avoids any bugs that might have crept in and that could pose a risk
to the stability of the released version.

The new version will be announced per the [announcement guidelines] in the release process documentation.

The [current release board](#current-release-board) will be closed, and all open tasks on it will be moved back to the
[backlog board](#backlog-board).
The tasks could then be considered for the next version, based on the [planning](#pre-planning) guidelines.

During the week when the general availability release is performed, the next version will be planned.
Additionally, a meeting to retrospect the last release cycle will be held.
There will be no dedicated [test day](#test-days), as the release candidate has been tested and no changes have occurred since.

### Unplanned Work

To be expanded

#### Ongoing Maintenance

To be expanded

#### Exception Process

To be expanded

### Test Days

To be expanded

[announcement guidelines]: ../release-process/#step-7-announce-release
