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

## Build Delivery
When new features or bug fixes are implemented, NTop will need to provide updated nProbe builds for Catchpoint on all supported platforms.  Currently the Catchpoint Endpoint Agent supports Windows and Mac.  When builds for Catchpoint are available, they can be uploaded to Releases in Github.  Catchpoint developers will download builds from here for further testing. 
