# AgGateway's ADAPT Data Model (ADM) standard issue management

## Introduction

This repo contains documentation and ADM-related issues. It does not contain code. The ADM-related issues are managed in a [GitHub project](https://github.com/ADAPT/ADM/projects/1). Each issue is in a state as specified below.

## Issue state diagram

[State diagram](https://app.creately.com/d/aciCyRbf6oy/view)

## Issue states

State | Score CC State | Description
--- | --- | ---
New | N/A | A submitter submitted the issue. The submitter may need to refine the issue content before it’s ready to transition `Discussion` or `Implementing`.
Discussion | N/A | The submitter would like to discuss the issue with the AC prior to creating/changing components in Score.
Implementing | WIP | The submitter has created/changed components in Score and those changes are in WIP (work-in-progress) status in Score.
Implemented | Draft | The submitter regards that work on components they created/changed in Score is complete and has changed the status in Score to Draft.
AC review | Draft | The submitter has the set of related issues (perhaps only one) ready to review with the ADAPT Committee.
Approved | Draft | An Architecture Committee review team has approved the issue.
Candidate | Candidate | The components associated with the issue are set to Candidate status in Score.
Reconsider | Draft or Candidate | A member of the AC believes that, in the interest of ADM quality, the issue should be reconsidered.
Member reveiew | Release | A draft release has been created in Score.
Ready for release | Release | The member review is complete with nothing left to process

## Issue transitions

From state | To state | Guard conditions (i.e., what must be true for the transition to occur)
--- | --- | ---
Start | New | - A submitter has an OAGIS issue to submit.
New | Discussion | <ul><li>The submitter has determined that he/she wants to discuss the issue (and perhaps related ones) with the AC prior to to creating/changing OAGIS components.</li><li>The submitter has properly formatted the issue</li><ul><li>The title is in the correct format.</li><li>The description in the correct format.</li><li>An appropriate milestone is specified.</li><li>Appropriate labels are set.</ul></ul>
