# Thesis Releases

Public distribution repository for Thesis for Windows. Application installers
and update packages belong in GitHub Releases, not Git history. No course
content or private development repository is published here.

Connect this repository to Netlify using Import an existing project. Select
`main`, leave the build command blank, and use `site` as the publish directory.
The root netlify.toml supplies that directory automatically.

The site is https://thesisreleases.netlify.app/. Version 0.1.3 is the bootstrap
release that pins its `/latest.json` feed and publisher's public signing key.
Versions 0.1.2 and earlier need one manual installation to enable site updates.

Upload and verify versioned GitHub release assets before updating `site/latest.json`.
Never overwrite versioned packages. Netlify publishes the small site directory
on a push to main; the signed manifest references the large files in Releases.
The application verifies the manifest and downloaded package hash before passing
it to Windows' updater. This is separate from Windows Authenticode signing.

Do not add private signing keys, credentials or course files to this repository.
