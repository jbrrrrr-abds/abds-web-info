---
{"dg-publish":true,"permalink":"/client-design-archive/step-3-accessing-submitted-design-lists/"}
---

Supabase - www.supabase.com

When Clients complete their selection in the Client Design Archive App and submit it successfully, the results are posted into a Supabase table.

The submissions will contain the following:

- "Company"
- "Account Email" - this is the email associated with the login that was used
- "Sender Email" - an optional field in case the actual author has a different email address than the login email
- "Designs" - this is a JSON-formatted text object that contains the information on the designs that were selected
	- Design image URL
	- Design name
- "Notes" - any optional notes that were input to accompany the submission

## Viewing Submissions

1. Log in to Supabase
2. Open the "Design Archive" project
3. Open the "client-design-submission" table

## Future Update:
- Provide a URL in the submission table entry that will generate a web page containing a visual list of the Client information and selected designs, which could then be saved as a PDF for later reference
- Create an automation that periodically fetches all new entries in the "client-design-submission" table and emails them to a designated user


back to  [[client-design-archive/index\|index]]