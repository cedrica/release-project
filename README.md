# Contact:
- ProductOwner: Cedric Leumaleu

## Versioning (How to read a Versionnumber):
- Major.Minor.Micro
- Micro: Is for bugfixes for example 1.0.1 | 1.0.2 | 1.0.3
- Minor: Is for development new features for example 1.1.0 | 1.2.0
- Major: Is for greater changes like API change and impact on user/customer side

# Release:

## manually (Git) :

1. create release-branch from develop (all features are merged in develop before)
2. change version in gradle.properties (remove -SNAPSHOT)

- The Version Number shall be formatted like this M.m.m
- Small Bugfixes shall increase the second minor by one.
- General Features shall increase the first minor by one.
- Severe changes / versios will affect the major, by increasing it.

3. change version in Installer/ib.install4j at all occurrence
4. update Release Notes - /<MY-PROJECT>/release/release_notes.txt
5. merge with master
6. set tag on commit (to master) (name is version from gradle.properties) - git tag "<version>" or via bitbucket UI
7. change version in gradle.properties (increase second minor Version by one and add -SNAPHSHOT) in develop-Branch
8. merge with develop

