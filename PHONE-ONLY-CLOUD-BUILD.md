# Build Virtual Abacus using only your Android phone

This project includes a GitHub Actions workflow that builds the debug APK on GitHub's hosted runner. No AndroidIDE or computer is needed, but you need a GitHub account and internet access. GitHub Actions usage limits/availability depend on your account and repository settings.

## Steps
1. Download and extract this ZIP on your phone.
2. In your phone browser, sign in at https://github.com and create a **new public repository** named `VirtualAbacus` (or use a private repository if your account allows Actions there).
3. Open the new empty repository. Tap **Add file → Upload files**.
4. Upload the contents inside the `VirtualAbacus` folder, including the hidden `.github` folder and its workflow file `.github/workflows/build-apk.yml`. If your mobile browser cannot select hidden `.github` files or upload folders, use GitHub Codespaces in the browser instead, or tell the assistant what options you see.
5. Commit the uploaded files to the `main` branch.
6. Open the repository's **Actions** tab and select **Build Virtual Abacus APK**. If asked, enable workflows, then tap **Run workflow**.
7. Wait for the run to finish. Tap the successful run and find **Artifacts → Virtual-Abacus-debug-APK**. Download the artifact ZIP.
8. Extract the artifact ZIP, tap `app-debug.apk`, and allow your browser/file manager to install unknown apps if Android asks.

## Troubleshooting
- If the Actions tab says workflows are disabled, enable Actions for the repository and run again.
- If the build fails, open the run and copy the first red error lines so they can be diagnosed.
- This produces a debug APK for personal testing, not a Play Store-signed release.
