# Catchpoint-NTop Git Hub

This repository is for tracking the joint effort of Catchpoint and NTop on the integration of Catchpoint's Endpoint Agent with NTop's network traffic analysis software, nProbe.  This README quickly overviews the usage of the Github repo, and how we will use it to track and manage this project.

## Reporting Issues

Issue reporting will be handled here through Github.  To report an issue, click the Issues tab in the upper left of the Github page, and click the green button labeled `New Issue`.  When filling out an issue, please provide as clear and concise issue title as possible.  When filling out the issue description, this should also be as clear and complete as possible, with the aim to provide the developer as much info and as clear a way forward as possible.  Finally, when reporting issues, the proper issue labels should also be attached to the issue. More info on labels is noted below.

## Issues: Label Types
When reporting issues, there are labels that should be associated with each issue to help the developers assess status, priority and issue type.  Each issue should have one of each label type associated with it.  The label types are as follows:

### Type
This label corresponds to the issue type.  An issue can be one of the following types:

- **Bug:** An issue was found not to be working correctly in an existing build.  When reporting a bug, steps to reproduce the bug should be made as clear as possible, preferably with numbered or listed steps if possible. 
- **Feature:** Add a brand new feature/functionality.  When reporting a feature, the requirements for the feature should be made as clear as possible.

### Priority
This label corresponds to the priority or urgency of the issue.  Priorities are in 1 of 3 levels:
- High
- Medium
- Low

### Status
This label corresponds to the current status of the issue.  Unlike the Type and Priority, Status is regularly changing, and should be updated when necessary to reflect the status of the issue.  Issue statues can be one of the following:
- **Open:** Issue is open and waiting implementation/fixing
- **In Progress:** Issue is currently being worked on
- **Waiting Review:** Implementation has been completed and is waiting review/testing
- **Complete:** Issue has been tested and verified
- **Canceled:** Issue was canceled or made invalid

## Build Delivery And Tracking

When new features or bug fixes are implemented, NTop will need to provide updated nProbe builds for Catchpoint on all supported platforms. Currently the Catchpoint Endpoint Agent supports **Windows** and **Mac**.  When new features or fixes are made, we will need to test and verify on both platforms.  Because of this, builds provided should be in sync (i.e. off the same git branch/tag and build/sha number). The process for build delivery and tracking would be the following:

1.  A bug or new feature request is reported to Git->Issues. The issue report should follow the guidelines laid out above.
2.  Developer takes the issue, implements a solution.
    * Developer places the Git Issue in "Waiting Review"
    * Developer uploads new build executable for all supported platforms (Windows/Mac) to Git Releases
    * Each build name should have the following format for tracking purposes: ntop_major.minor.build. The builds for each platform here should be identical.
    * Uploading the build to Releases should also come with a set of release notes, which provides a numbered list of changes, referring to the Git issue number that the build addresses.
3.  Tester will download the build and test the Issues that the build addresses.
    * If Issue appears resolve, tester should move on to #4.
    * If an Issue still occurs or is incomplete, the tester should place the Git Issue back to the "Open" status, and comment in the issue further what still needs to be done. This should be clear and thorough enough for the developer to pick right back up.
    * Developer should confirm that re-opened issue is in fact valid. If the re-opened issue is valid, the developer should remove the previously uploaded build, and re-upload a new build when a new fix/implementation is complete.
4.  If the build addresses all newly Open reported issues, the tester should mark all "Waiting Review" issues as "Complete", and close the issue out.


