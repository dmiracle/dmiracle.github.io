---
title: "Typical Issue"
date: 2021-11-11T04:00:45-06:00
draft: true
---

Testing an SDK fix showed no change in error output. Checking the update showed no version bump, no update had been performed.  
Go check the release. The release shows up on github, check the artifact build. Build failed, no release artifact available to install. Look at failed release. It is trying to publish the old version, not the new version.  
Check that all manual updates are done. Check release. Release looks normal until

Release commit is showing a previous hash -- tagged to the commit from the last release. Likely because the release was deleted without deleting the tag `git push --delete origin v0.1.10