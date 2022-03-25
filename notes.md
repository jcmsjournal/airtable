# Airtable thoughts

## Here is the workflow, more or less

### Open Submission
An Author submits an Article via open submission

The Article enters Desk Review

The Article is desk reviewed by an Assistant Editor.
The Article is either:
	Accepted into Pre-Review
	Rejected, with an optional note by the Assistant Editor

### Facilitated Submnission
An Author submits an article via facilitated peer review by filling out the form.

The Article enters Pre-Review

{!-- Here is where we begin --}
### Pre-review
An Article enters Pre-Review
Its status is Awaiting Reviewers
The Editor or Associate Editor assigns Proposed Reviewers
The Editor or Associate Editor changes the article status to COI Pending

The Managing Editor performs a COI Check

The Article's Proposed Reviewers either:
	Passe the COI Check. The Managing Editor changes the Article's Status to Into Review.

	Fail the COI Check. The Managing Editor changes the Article's Status to Awaiting Reviewers.

### Review Requests
The Managing Editor creates a Review Request for two Reviewers.

The Editor enters an optional note to be included with the Review Request.

The Reviewer receives an email with a link to a form to either Accept or Reject the Review Request. The email includes the Article's title, key words, and abstract. They are given two weeks to Approve or Reject the Review Request.

The Reviewer clicks on that link and either:
	Approves the request. The Article is moved to Under Review.
	Rejects the request. The Managing Editor receives an email. The Managing Editor either:
		Creates a Review Request for an alternate reviewer that has passed COI Check.
		Moves the Article's status in Pre-Review to Awaiting Reviewers.

The Reviewer does not click on that link for a week:
	JCMS Bot sends out a reminder email with the same link

The Reviewer does not click on that link for another week:
	JCMS Bot changes the Review Request to Ignored. The Managing Editor receives an email. The Managing Editor either:
		Creates a Review Request for an alternate reviewer that has passed COI Check.
		Moves the Article's status in Pre-Review to Awaiting Reviewers.

### Under Review
The Reviewer receives an email with the Article's title, key words, abstract, manuscript, and a link. They are given four weeks to complete a review.

After three weeks, the Reviewer receives a reminder email with the link.

After four weeks, the Reviewer receives a reminder email with the link.

The Reviewer clicks on the link and submits their Reader Report, and the Article moves into Awaiting Decision. The Editor receives an email.

After six weeks, the Reviewer receives a reminder email with the link and a warning that the review will be canceled if it is not received within two weeks.

After eight weeks, the Review is canceled. The Reviewer receives an email notifying them. The Editor and Managing Editor receive emails. The Managing Editor either:
		Creates a Review Request for an alternate reviewer that has passed COI Check.
		Moves the Article's status in Pre-Review to Awaiting Reviewers.

{!-- Here is where we end --}

### Awaiting Decision
The Editor makes a decision. The Editor also fills out a note to the Author. which is either:
	Accept. The Author receives an email and the Article is forwarded to Publication Queue.
	Reject. The Author receives an email.
	Revise. The Author receives an email with a link to a form to submit a Plan for Revision.

(Questions here: How to handle Editorial revisions of Reader Reports? How to handle requests from the Editor for a Reviewer to redo their Reader Report?)

### Revision Plans
The Author receives an email with anonymized Reader Reports and the Editor's Note, and a link to submit a Plan for Revision. They are given four weeks to submit their Plan for Revision.

After three weeks, the Author receives a reminder email with the link.

The Author clicks on the link and fills out their plan for revision. The Associate Editor receives an email.


