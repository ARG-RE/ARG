ACRES REALTY GROUP — GOOGLE SHEETS LEAD CAPTURE SETUP

FILES INCLUDED
/scan/index.html
/350_Grove/index.html
/assets/ARG-horizontal-transparent.png
/google-apps-script/Code.gs

EXPECTED URLS
https://www.acresrealtors.com/scan/
https://www.acresrealtors.com/350_Grove/

GOOGLE SHEETS SETUP

1. Create a new Google Sheet.
2. Name it something like "Acres Realty Group Leads."
3. In the Sheet, go to Extensions > Apps Script.
4. Delete the starter code.
5. Paste the contents of google-apps-script/Code.gs.
6. Click Save.
7. Click Deploy > New deployment.
8. Choose "Web app."
9. Set:
   - Execute as: Me
   - Who has access: Anyone
10. Click Deploy and authorize access.
11. Copy the Web App URL ending in /exec.
12. Open /350_Grove/index.html.
13. Find:
    const GOOGLE_SCRIPT_URL = 'PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE';
14. Replace the placeholder with your Web App URL.
15. Upload the site folders to your website.

THE SHEET WILL STORE
Timestamp
Property
Property Slug
Name
Email
Phone
I'm Looking To
Source
Page URL

PROPERTY TAGGING
Each property page carries its own hidden property name and slug.
For 350 Grove:
Property = 350 Grove Street
Property Slug = 350_Grove

When creating another property page, copy the folder and update:
- page title and visible property text
- hidden input "property"
- hidden input "property_slug"
- the sessionStorage key if desired
