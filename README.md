# Suresh Nalla — SAP BASIS Portfolio

This version has one source of truth: `data/site-data.js`.

## What is new

- The portfolio website reads professional information from `data/site-data.js`.
- `resume.html` uses the **same data file** and automatically builds a resume in the same simple, text-focused style as the previously attached resume.
- From the website, **Resume** opens the generated resume.
- On the resume page, **Print / Save as PDF** uses the browser print dialog. Choose **Save as PDF** to create a PDF whenever you need an updated copy.
- You do not need to edit `resume.html` when your counts, experience, certifications, skills, achievements or education change.

## Updating your details

For normal updates, edit only:

`data/site-data.js`

Examples:
- `stats.serviceRequests`
- `stats.incidents`
- `stats.experience`
- `profile.summary`
- `currentRole`
- `experience`
- `certifications`
- `skills`
- `achievements`
- `education`
- `blogPosts`

The portfolio and resume will use the updated values automatically.

## GitHub Pages setup

Recommended repository name:

`YOUR-GITHUB-USERNAME.github.io`

GitHub Pages can host this as a free public website on GitHub Free.

After creating your GitHub account:

1. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`.
2. Upload all files/folders from this package, preserving the `data` folder.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. Your site will appear at `https://YOUR-USERNAME.github.io/`.

Publishing can take a few minutes.

## Important privacy note

The original resume contains a phone number. This website intentionally does **not** publish the phone number, and the phone number has been removed from the public website data source.

## LinkedIn and GitHub

Replace the placeholder URLs in `data/site-data.js`:

- `profile.linkedin`
- `profile.github`

Once you create the GitHub account, your GitHub URL will look like:

`https://github.com/YOUR-USERNAME`

Your website URL will look like:

`https://YOUR-USERNAME.github.io/`


## Automatic resume download

The **Download Latest Resume (PDF)** button does not use a stored PDF file.

When a visitor clicks it:
1. The current `data/site-data.js` is loaded.
2. `resume.html` builds the resume from that data.
3. The page generates a fresh A4 PDF in the visitor's browser.
4. The PDF is downloaded as `Suresh_Nalla_Resume.pdf`.

Therefore, when you update the data file and publish the website, future downloads automatically contain the latest information.

The phone number is not stored in the public website data and is not rendered anywhere on the public website or generated resume.

The PDF generator is loaded from the public `html2pdf.js` CDN when the resume page is opened.


## Final clean version
This package is the clean public version for GitHub Pages: no sample blog posts and no phone number in the public data source.


## Published Blog

The first real article is available at:

`blog/what-is-sap-basis.html` — **SAP BASIS: The Invisible Force Behind SAP**

Future articles can follow the same structure and be added to the `blog/` folder, then linked from `data/site-data.js`.
