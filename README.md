# AgGateway's ADAPT Data Model (ADM) standard issue management

## Introduction

This repo contains documentation and ADM-related issues. It does not contain code. The ADM-related issues are managed in a [GitHub project](https://github.com/ADAPT/ADM/projects/1). Each issue is in a state as specified below.

## Issue state diagram

[State diagram (maintained in external application)](https://app.creately.com/d/aciCyRbf6oy/view)

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
Start | New | <ul><li>Submitter has an issue to submit.</li></ul>
New | Discussion | <ul><li>Submitter has determined that he/she wants to discuss the issue (and perhaps related ones) with AC prior to to creating/changing components.</li><li>The submitter has properly formatted the issue</li><ul><li>The title is in the correct format.</li><li>The description in the correct format.</li><li>An appropriate milestone is specified.</li><li>Appropriate labels are set.</ul></ul>
New | Implementing | <ul><li>Submitter has properly formatted the issue (see `New` to `Discussion`)</li><li>Submitter is ready to create / change components in Score and those components are in WIP status in Score.</li></ul>
Discussion | Implementing | <ul><li>Same as `New` to `Implementing`</li></ul>
Implemented | AC review | <ul><li>Submitter is ready to review with AC.</li></ul>
AC review | Implementing | <ul><li>AC rejects the issue.</li></ul>
Implementing | Implemented | <ul><li>Submitter regards that work on components they created/changed in Score is complete and has changed the status in Score to Draft.</li></ul>
AC review | Approved | <ul><li>AC approves the issue.</li></ul>
Approved | Candidate | <ul><li>Components associated with the issues have been set to Candidate status in Score.</li></ul>
Candidate | Reconsider | <ul><li>An AC member believes that, in the interest of quality, the issue should be reconsidered.</li></ul>
Member review | Reconsider | <ul><li>Same as `Candidate` to `Reconsider`</li></ul>
Reconsider | Implementing | <ul><li>AC reverses its earlier approval.</li></ul>
Member review | Ready for release | <ul><li>Members have validated the release.</li><li>All issues have been processed from the member review.</li></ul>
Ready for release | End | <ul><li>ADM is released and the issue is closed and archived.</li></ul>
