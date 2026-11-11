# Personal rclone OAuth site

Public information pages for a **personally operated rclone / Google Drive OAuth client**. This is not an official rclone or Google project. The website does not contain OAuth credentials or handle user authentication.

## Publishing with GitHub Pages

1. Open **Settings → Pages** in this repository.
2. Set **Source** to **Deploy from a branch**.
3. Choose **main** and **/(root)**, then **Save**.
4. After deployment, visit the site and check that the privacy and terms pages load.

Expected GitHub Pages URLs (only work after Pages is enabled):

- Homepage: https://op06072.github.io/rclone-oauth-site/
- Privacy: https://op06072.github.io/rclone-oauth-site/privacy.html
- Terms: https://op06072.github.io/rclone-oauth-site/terms.html

Set these addresses under **Google Auth Platform → Branding** only after the URLs are publicly accessible. Confirm the domain ownership / Search Console verification requirements for your OAuth use case. Publishing to a GitHub Pages subpath alone **does not guarantee** Google domain verification or acceptance.

## Data handling

The OAuth flow takes place through Google and locally installed rclone. This repository hosts only static HTML and CSS; it does not contain a Google Client ID, Client Secret, OAuth token or backend service. The privacy policy describes access to Google Drive metadata and contents, local OAuth token storage, and local VFS cache behavior.

The policy reflects **personal, local use**, not a public cloud storage service. Update it if the actual handling of data changes.

## Files

- `index.html` — public homepage and functionality overview
- `privacy.html` — privacy policy and Google user data handling
- `terms.html` — terms and project disclaimer
- `style.css` — responsive stylesheet

## Security

Never commit `rclone.conf`, OAuth tokens, client secrets, or personal Drive contents to this repository.
