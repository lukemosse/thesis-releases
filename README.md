# Thesis Releases

Public distribution repository for Thesis for Windows. Application installers
and update packages belong in GitHub Releases, not Git history. No course
content or private development repository is published here.

Connect this repository to Netlify using Import an existing project. Select
`main`, leave the build command blank, and use `site` as the publish directory.
The root netlify.toml supplies that directory automatically.

The update feed is not live yet. Once the final Netlify URL is known, a new
installer will pin that URL and the publisher's public signing key. Signed
latest.json will be deployed only after the referenced release assets exist.

Do not add private signing keys, credentials or course files to this repository.
