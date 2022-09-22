# Readers and Reports Documentation

Readers and Reports manages the peer review process.

### Step 1: The Managing Editor brings an article into the peer review queue.
Once the Managing Editor changes the status of a submission to "Sent into review," the article is automatically imported into the Readers and Reports app.

However, re-submissions are _not_ imported automatically. In that case, the Managing Editor will navigate to the Articles table, and the Kanban view, and add a record in the "Awaiting reviewers" stack. They will enter the information for the article: title, keywords, abstract, manuscript, and also search for the original article record that this is a resubmission of.

### Step 2: The Editor selects peer reviewers.
Whenever (and however) an article enters "Awaiting reviewers," the Editor receives an email letting them know an article is awaiting reviews (with a direct link). Or, the Editor can navigate to the Kanban view in Article and see all the articles awaiting reviewer selection.

The Editor opens the record with the title, abstract, etc., and can read the manuscript online or download it. From that view, they can search the Reviewer database and select them, or create a new record for a reviewer.

The Editor selects Reader 1, Reader 2 (no particular ordering here, we just need different fields), and then Alternate Readers (as many as you'd like). Once the Editor does this, they change the status of the Article to COI Check.

#### Adding Reviewers to the database
There are two ways to add reviewers to the database:

* Add while doing a Reviewer search for an article. When the Editor clicks on the "+ Add a record" button in the Article record for Reader 1, Reader 2, or Alternat Readers, Airtable will bring up a search box. The editor can search for Reviewers (by name or by field or by institution). Or, they can click the "+ Add new Record" at the bottom, and enter the information directly from there.

* Add a Reviewer directly to the Reviewers table. Navigate to the table. Click on the "+" button either below the last record in the Reviewers table, or the "⨁" button at the bottom left of the Reviewers table, in the footer row. Clicking on the "↔" button (set diagonally) in the ID column will expand a record to make data input easier.

### Step 3: The Managing Editor performs a COI check.
The Managing Editor looks up the Article in the Sumbissions Portal base, and confirms there are no COIs with the proposed Readers.

**If there are conflicts**, the Managing Editor deletes the Readers in question, and leaves a helpful note in the comments for the Editor, and changes the status back to "Awaiting reviewers". The Editor receives an email, rinse, repeat.

**If there are no conflicts**, the Managing Editor changes the status of the Article to "Ready for review."

### Step 4: Soliciting reviews
When the Managing Editor changes the status of the Article to "Ready for review," the app creates two new Review Requests for the two Reviewers in the Reader 1 and Reader 2 fields of the Article. Their status is automatically generated as "Awaiting Editor's note." The Editor receives an email alerting them, with a direct link to the record.

The Editor then enters an optional personalized note to the Reviewer in question that will be included in the email request. Once they have done that for a review (or not), they change the status to "Request pending." As soon as they do that, the app generates an email to the Reviewer requesting a review. This email contains: the Article title, abstract, keywords; a request that they accept or decline the review within a week; a guideline that reviews are due 4 weeks after they are accepted; and a link to submit their response.

**If the Reviewer accepts the request**, the app automatically sends an email to the Reviewer with: the Article title, abstract, keywords, and manuscript; a deadline for the review in four weeks; and a link to submit their reader report.

**If the Reviewer declines the request**, the Managing Editor receives an email notifying them, that includes a link to the Article record. From there, they manage soliciting another reviewer, either by promoting a reviewer from the "alternate" Readers in the record, or by changing the status back to "Awaiting reviewers," for the Editor to select additional readers.

**If the Reviewer ignores the request**, they will receive a reminder email after one week. If they ignore the request for two weeks, the app will cancel the review request, and send a notification email to the Managing Editor that includes a link to the Article record. From there, they manage soliciting another reviewer, either by promoting a reviewer from the "alternate" Readers in the record, or by changing the status back to "Awaiting reviewers," for the Editor to select additional readers.

### Step 5: Submitting Reviews.
As soon as a Reviewer accepts a Review Request, the app emails them with the article and a link to submit the review, with a timeline of four weeks.

When the review is prepared, the Reviewer will click on the link in the email and submit their Review. They assign assessments of "Exceptional," "Solid," "Needs work," or "Inadequate" in each of the following categories: Overall Quality; Salience to Specialists; Interest to the Broader Field; Quality of Research & Method; Significance of Claim, Diversity of Ideas, and Originality of Research; and Quality of Writing. They will also submit a written report by uploading a file a Word file. They can also upload a manuscript with marginal comments. It also allows: a confidential note to the editor; a checkbox to opt in to having their name disclosed; and checkbox to opt out of reviewing a revised resubmission.

#### Changing Review deadlines
All JCMS Bot emails all have a reply-to of editors@jcmsjournal.org. If Reviewers wish to negotiate timeline, they may reply to the JCMS Bot email (the email will say as much). Airtable, sadly, is not really smart enough to make it easy to input a new due date, and the JCMS Bot will email the Reviewer after three and four weeks. That said, it's easy to make a note of a new due date in the comments on the Review Request.

### Step 6: Rendering a decision
Once an Article receives two Reviews, the Editor receives a notification that the Article is ready for a decision, with a link to the Article record. The Reviews can be viewed by navigating to them through the record. You will be able to navigate to them through the Review Requests field, which will include all Review Requests made for that article, they will include links to the submitted Reviews where present. The Editor now has enough information to render a decision, or strike a decision committee.

## Revisions
A piece that's given a decision of Revise & Resubmit

### Step 1: 

### And beyond...?

And this is where I have workflow questions, which we don't really have answers for yet. The full Reviews are very easily made available for a review committee, and the blinded review for author view is a bit less easy. The Readers & Reports base (by design) does not have any identifying author information. Decision in hand, the time has come to communicate with the author.

I believe, likely, the best way to do this is high-touch and low-automation. The Managing Editor prepares the Reviews for the Author by downloading the Reader Report rubrics for each of the readers, as well as the attachments, and anonymizes them. They will then send the Editor an email with the Reports and author contact info. The Editor will then write an email to the Author informing them of the decision.

The Submissions Portal Submissions table has a "decision" field, which the Managing Editor should update when appropriate: "Desk reject," "Reject," "Revise," and "Accept."

The Author will send the revised manuscripts to the Managing Editor, who will upload revised artilces into the Readers and Reports app.