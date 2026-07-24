# Installation

1. Extract the ZIP.
2. Copy every extracted file and folder into the root of the `sabry134` profile repository.
3. Keep the folder structure unchanged.
4. Commit and push the files.
5. Create a GitHub personal access token.
6. Open the profile repository settings.
7. Go to `Secrets and variables`, then `Actions`.
8. Create a repository secret named `METRICS_TOKEN`.
9. Paste the personal access token as its value.
10. Open the `Actions` tab.
11. Select `Generate Cyber Metrics`.
12. Run the workflow manually once.

The first workflow run creates `github-metrics.svg` in the repository root.

## Included files

```text
README.md
SETUP.md
assets/
  cyber-header.svg
  cyber-footer.svg
.github/
  workflows/
    metrics.yml
```

## Important

The README no longer uses `github-profile-summary-cards.vercel.app`, which was producing the red rate-limit cards.

The GitHub metrics image is generated inside the repository and refreshed automatically once per day.

The browser console errors mentioning `content.js`, `feature.js`, `vendor.js`, or `window.Feature` are generally injected by a browser extension and are separate from the README.
