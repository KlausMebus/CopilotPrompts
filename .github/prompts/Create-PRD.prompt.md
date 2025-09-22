---
mode: agent
tools: ['createFile', 'search', 'fetch']
---

# Product Requirements Document (PRD)

## General Information

The naming convention for the documents is as follows:
- [Name]-[Version].md where the [Version] starts from 0001 and increments for each new version of the document.

**Always** use the latest version of each document.


## Workflow

* Create a PRD for a new product based on an Idea Document.
* The Idea Document is default `idea-xxxx.md` in the `docs` folder (where `xxxx` is the version number of the Idea Document). Always use the highest version number (latest version). If the Idea Document does not exist then ask for a location for the Idea Document.
* The PRD should include the following sections:
  * Title with a short title of the product and "(PRD)" suffix
  * Description: A brief overview of the product and its purpose.
  * Problem Statement
  * Goals and Objectives
  * Target Audience
  * Features and Requirements
  * User Stories for all features
* The PRD should be saved in markdown format in a file `prd-xxxx.md` in the `docs` folder (where `xxxx` is the idea ID).