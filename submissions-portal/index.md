# Submissions Portal Documentation

The Submissions Portal pulls together two parts of the article pipeline: author submission of manuscripts, and desk review.

## Author submission
The author submission form is here: https://airtable.com/shr9RXgxBFJoaD6O1. It accepts all the information required for a submission (author name, email, institutional affiliation, bio; article title, abstract keywords, manuscript). The form does not limit the manuscript to a particular format, so it is possible that authors will submit manuscripts in formats we're not prepared to accept. The Assistant Editors will have to correspond with the author (and can do so by desk rejecting the piece).

### Steps

#### 1. The author navigates to the form
The author will navigate to the form from the JCMSJournal.org website. (https://jcmsjournal.org/submit will take users to the submissions page on JCMSJournal.org.) They will fill out the form.

#### 2. The author submits the form
When the author clicks submit. They see a confirmation screen. Four additional things happen:

1. The information they've submitted is captured into the "Submissions" table in the Submissions Portal base.
2. A record is automatically created in the "Desk Reviews" table in the Submissions Portal base.
3. An email is sent to the author confirming receipt of their manuscript. (TODO: this email is currently a stub; write a real email.)
4. An email is sent to the Assistant Editors notifying them a new submission has arrived. There is a link to the Desk Reviews record.

#### 3. The Assitant Editors peform desk review
The Assistant Editor can do one of two things:

1. Log in directly to AirTable and navigate to the Desk Reviews table, and then to the "Board view, by status" view. That will give them a kanban-style view of all articles in Desk Review. There are three statuses: Awaiting desk review; Forward to peer review; and Desk reject. Any new submissions will be in the Awaiting desk review stack. Clicking on the card will open the record. Or,
2. Click on the link in the email. This will automatically take the Assitant Editor to the record.

The record view will show a record of the submission. It includes: title, author, email, keywords, abstract, and manuscript. There are four fields of especial interest. If one clicks on the "Submitted manuscript," the manuscript is loaded in the browser window, or can be downloaded.

At the very top, "Assigned to". This is optional; if the Assistant Editors wish to use this field, they can assign the record to either of them. TODO: coordinate with Assistant Editors if they wish to use this feature; and create assigned-by views.

##### Desk review decisions
There are then "Notes for author (when rejected)",  "Anonymized manuscript", and "Status". They are used to render decisions as follows:

**If the piece is a desk reject,** the Assistant Editor writes notes in "Notes for author (when rejected)". What they write will be included in the email to the author. They then change status from "Awaiting desk review" to "Desk reject". As soon as they do that (so be careful!--this is a finalizing action, no confirmation buttons or anything), an email is sent to the author. If they do not enter anything in the "Notes for author (when rejected)" field, the email is sent, but without any personalized note. (This could well be the place where any authors whose manuscripts are in the wrong format may be notified of that fact, and be invited to resubmit the piece using a Word document.)

**If the piece is accepted into peer review,** the Assistant Editor downloads the manuscript, and anonymizes it. Once that is done, the Assistant Editor uploads the anonymized manuscript by dragging it to the "Anonymized manuscript" field, or using the uploader (i.e., "Drop files here or browse"). They then change the status from "Awaiting desk review" to "Forward to peer review".

If the Assistant Editor changes the status to "Forward to peer review" without uploading an anonymized manuscript, it will show up in the "Awaiting anonymization" view. 

Weekly reminder emails are sent to the Assistant Editors detailing any submissions that are "Awaiting desk review" or "Awaiting anonymization".

#### 4. A piece enters peer review
Once a piece is "Forward[ed] to peer review" and has a file uploaded to its "Anonymized manuscript" field, the submission is added to the "Pre-review" table. The Managing Editor receives an email notifying them that a piece is ready to go into peer review.

The Managing Editor downloads the anonymized manuscript, and creates a record in the Readers and Reports app. This will require manual re-entry of: article title, abstract, keywords, and anonymized manuscript. That workflow is detailed in [the Readers and Reports documentation](../readers-and-reports/index.md).

