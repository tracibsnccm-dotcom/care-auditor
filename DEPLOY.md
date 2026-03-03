# Deploying the C.A.R.E. Clinical Sequencing Auditor

## Fixing "404 Page Not Found" when clicking the Auditor button

The 404 happens because the **link on your main website** is pointing to the wrong URL. The button that opens the auditor must point to the **exact location** where you uploaded these files.

### What to do

1. **Note where you uploaded the auditor files**  
   Examples:
   - `https://yoursite.com/care-auditor/`
   - `https://yoursite.com/auditor/`
   - `https://yoursite.com/tools/clinical-sequencing-auditor/`

2. **Update the link on your main website**  
   Find the button or link that says something like "Auditor", "Clinical Sequencing Audit", or "Begin the Audit". Set its URL to one of:
   - `https://yoursite.com/care-auditor/` (if the folder is `care-auditor`)
   - `https://yoursite.com/care-auditor/index.html` (same folder, explicit file)

   Use the same domain and path you used when you uploaded the HTML.

3. **If you're not sure of the path**  
   Open the auditor by going directly to the URL where you uploaded it (e.g. in your hosting file manager, open `index.html` and copy the address from the browser). Use that full URL as the button link.

### Files to upload together (same folder)

- `index.html` (main auditor)
- `explainer.html` (optional overview page)
- `app.js` (required for index.html)

### Relative links inside this project

- `explainer.html` links to `./index.html` — so `explainer.html` and `index.html` must be in the **same directory** on the server.
