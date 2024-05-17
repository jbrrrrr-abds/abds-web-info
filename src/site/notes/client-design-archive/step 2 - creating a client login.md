---
{"dg-publish":true,"permalink":"/client-design-archive/step-2-creating-a-client-login/"}
---

Supabase - www.supabase.com

Supabase is a platform to host simple database structures without needing to administrate them internally.  It offers basic functionality like authorization, which is what is in use for the Client Design Archive App.

Each client that has a Design Archive Page in Prismic needs to have a login assigned in Supabase.  This is what will allow them to log in to the App.

For now, the process is to create the login manually for the Client, and provide them their login details by email or phone. 

1. Log in to www.supabase.com with the ABDS account.  This account has full administrative privileges to create/read/update/delete in the databases
2. Open the Design Archive project
3. Click on "Table Editor"
	1. There are two tables here related to the Client Design Archive App.  "Users", and "Client Design Submissions" - this is where the completed selections are sent to when the Client makes design selections in the App.
4. Open the "Users" table
5. Click the "Insert" option
6. Fill out an entry for the Client:
	1. **"email"** - this is what will be used to log in to the App
	2. **"pass"** - set this for the Client
	3. **"prismicSlug"** - this value is automatically generated when a Prismic Design Archive Page is created - copy that value here.  It should be the Client business name, all lowercase, with hyphens instead of spaces *(ex: "client-company-name")*
	4. **"company"** - enter the name of the Client's company.  This is only used when looking at the completed submissions, in the event that the email address that is used for the Client doesn't reflect their company.
	5. Test this login by trying it yourself in the Client Design Archive App
	6. Provide this login to the Client

## Forgotten Passwords and Broken Logins

If the Client reports that they've forgotten their password, or that the login is not working as expected, use the steps above to find the Supabase entry in the "Users" table for the Client's email address that they are trying to use, and change the password.  Test logging in to the App, and if it works, provide this to the Client.

## Multiple logins for the same Design Archive

Multiple logins can be created for the same Design Archive if necessary.  Follow the above steps, and make sure that the "prismicSlug" and "company" fields are the same for each login that is created for the Client.

When a submission is successfully posted over, it will contain the email address of the account that was in use when it was made, so that it will be possible to identify who generated the submission.  It also provides a field to enter a different email address before sending, so companies can share one login between multiple people but still have identification for who the exact author was.

back to  [[client-design-archive/index\|index]]