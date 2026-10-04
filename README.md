# Jefferson Kunkle Live Portfolio

This site is designed to read live content from the Google Sheet backend:

https://docs.google.com/spreadsheets/d/1i4FEtpV1uaH1DgivTYK0SWlfl--ecfkCcy8pgWlxLeg/edit

## How updates work

The site reads three tabs on each page load:

- `Site Settings`
- `Projects`
- `Photos`

Change the Sheet, refresh the website, and the content changes automatically.

### Photos tab

Use these fields:

- **Show?**: TRUE/FALSE
- **Project**: must match the Project Name in the Projects tab
- **Phase**: PRE or POST
- **Category**: Exterior, Kitchen, Bathroom, Landscaping, etc.
- **Caption**
- **Display Order**
- **Image URL**: publicly accessible HTTPS image URL
- **Source / Notes**: internal editing notes; the website does not display this field

## One-time Google setting

The spreadsheet must be accessible to public visitors for the website to read it.

In Google Sheets:

1. Open the backend Sheet.
2. Click **Share**.
3. Under General access choose **Anyone with the link**.
4. Set it to **Viewer**.

Only this dedicated portfolio backend should be public. Do not put private questionnaire or salary information in it.

## GitHub Pages

Put `index.html` in the root of a public GitHub repository and enable GitHub Pages from the default branch/root.

After that, the GitHub Pages URL stays the same while Sheet edits update the content dynamically.