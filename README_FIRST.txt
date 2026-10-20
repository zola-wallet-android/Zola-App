ZOLA WALLET — ANDROID CLOUD BUILD STARTER

This is a starter Android WebView app that opens https://zola.gt.tc/login.php. It does not modify your PHP website or database.

HOW TO BUILD USING YOUR ANDROID PHONE:
1. Create a GitHub account (if you do not already have one) and create a NEW PRIVATE repository named zola-wallet-android.
2. Upload the contents of this ZIP into the repository root, preserving folders and file paths.
3. Open the repository's Actions tab and enable Actions if prompted.
4. Select “Build signed Zola Wallet APK”, tap “Run workflow”, then run it on the main branch.
5. When it finishes successfully, open that workflow run and download the artifact named “zola-wallet-release”. It contains the signed APK and a private signing backup ZIP.
6. Keep the signing backup ZIP in a safe private location. It contains the signing key and credentials needed for future app updates. Never publish it or send it to anyone.
7. Download the APK on your Android phone, open it, and approve Android's “install unknown apps” prompt for the browser/file manager if asked.

IMPORTANT:
- This is a basic WebView wrapper; it relies on internet access and the website being available.
- It is a first build template and must be tested on your phone before public release.
- The workflow generates a fresh signing key for the first build. Do not rerun the workflow to make an update unless you restore the same signing key and credentials from the backup; otherwise Android may reject the update over the old app.
- Keep the GitHub repository PRIVATE while handling signing materials.
