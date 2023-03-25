# Programming/Support Documentation

Prepared 2022-10-26 by Scott Richmond.

## Preamble
The set of Airtable bases includes: Submissions Portal, Resubmissions Portal, Readers and Reports, and Post-Submission Pipeline. Each of these manages a different set of processes for the journal. The names are basically descriptive.

They also have differing levels of complexity: the Readers and Reports base manages the complex and conditional-heavy workflow of soliciting and receiving reader reports. The Post-Submission Pipeline, by contrast, is merely record keeping and includes no logic whatsoever.

## Basic Infrastructure
Where there is conditional logic, the most common way of accomplishing this is to create an Airtable View that filters by conditional logic, and to use the automation trigger "When a record enters a view" to do any automated actions.

Much of the time (but not all of the time), the Views in question filter on a Status field, the changing of which is the user action that sets off software action. (This also allows for user-friendly Kanban views.) For example, changing the status from "Awaiting Reader Selection" to "COI check" is what changes assignments and sends an email to the managing editor that a COI check is required. Because of this, the idiom for users is that "changing a status is taking an action."

We can separate the kinds of actions taken into a few different categories:
* Sending emails:
	- to team members, notifying them of action to be taken
	- to team members, giving summaries of various pipelines
	- to authors, notifying them of desk review decisions
	- to readers, soliciting, reminding, or sending info about reviews
* Creating records in other tables
* Archiving completed or otherwise old records

## Bases

### Submissions Portal
The Submissions Portal is for new blind submissions.