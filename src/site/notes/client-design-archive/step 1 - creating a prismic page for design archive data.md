---
{"dg-publish":true,"permalink":"/client-design-archive/step-1-creating-a-prismic-page-for-design-archive-data/"}
---

Prismic - www.prismic.io

1. Log in to prismic.io under the info@abds.co account, and open the Client Design Archive repository.
2. Create a new page, using the "Client Design Archive Page" type.
3. Input the Client Name field, and notice that the "page-slug" field is automatically generated with a unique identifier.  This is the key that the App will reference to fetch the appropriate data for this client.

At this point, you can save and publish, and the page will be available for the App to reference once the page slug is assigned to a Supabase login.

## input design data for this client
Each Client Archive Page uses a repeatable content type in Prismic called a "Design Unit".  These Design Units consist of:
**- Design image** (mandatory)
*- Design name*
*- Description of the design*

Inputting all of this data does not necessarily mean that all of it will display in the App - that is determined by how the App display template is currently coded.  The name and description fields are optional in case they are wanted in the future - only the image itself is necessary, but note: **if you do not input a name for the design, the image is the only connection between the picture that the Client sees and anything existing in the NetSuite ordering system world.  The design name doesn't need to be Client-facing - you can use something that is only for internal reference as long, as it helps relate the image that is uploaded to an actual item type in the NetSuite backend.  At minimum, a rough description of the design and primary colors would be recommended.**

Make sure save and **PUBLISH** when any edits are made.  If the page is not published, the new data will exist in the Prismic Admin but won't be available in the Client Design Archive App.







back to  [[client-design-archive/index\|index]]