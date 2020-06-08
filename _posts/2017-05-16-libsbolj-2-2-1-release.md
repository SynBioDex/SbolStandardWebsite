---
id: 2277
title: libSBOLj 2.2.1 Release
date: 2017-05-16T21:28:11+00:00
author: Tramy Nguyen
layout: post
guid: http://aries.ncl.ac.uk/sbol/?p=2277
permalink: /libsbolj-2-2-1-release/
categories:
  - Announcements
---
We are pleased to announce the release of libSBOLj-2.2.1 which is available for download from the [libSBOLj github repository](https://github.com/SynBioDex/libSBOLj/releases).

IMPORTANT NOTE: this supersedes libSBOLj-2.2.0 which has a significant bug in createRecursiveCopy. Anyone using libSBOLj-2.2.0 is encouraged to update to this version immediately.

This version of libSBOLj is also available from Maven Central. This release includes JAR files both with and without dependencies, as well as JAR files that include sources and javadocs for development. This release continues to include the old libSBOLj-deprecated.1.0.0 library. However, it likely will be the last release that does, so developers are strongly encouraged to migrate to SBOL 2 and libSBOLj-2.2.1 as soon as possible. A significant new feature of this version of the library is the addition of methods to directly search, obtain designs from, and submit designs to instances of SynBioHub repositories.

Links to the github repository, this release, an issue tracker, javadocs, a getting started tutorial, example code, and our email list for support can be found on the [SBOL website](http://sbolstandard.org).

Finally, we would like to hear from you. If you develop a tool that uses this library, please let us know, so we can advertise this on the SBOL website. Please fill out the following software [survey](http://sbolstandard.org/software/tools/).