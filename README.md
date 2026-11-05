# Pagora privacy policy

GitHub Pages site for the Pagora app's privacy policy.

- English: https://pqzmggg.github.io/pagora-privacy/ (`index.html`)
- Korean: https://pqzmggg.github.io/pagora-privacy/ko/ (`ko/index.html`)

Pages setting: Deploy from a branch, `main`, `/ (root)`.

## On-device AI model list

`models.json` lists the small language models the Android app can download when Gemini Nano is not available.
The app checks it once a day and offers an update when the highest-priority model for its version differs from the installed one.

- `id` must change whenever the model changes (books classified by the old `id` are classified again).
- `url` must be https. Fill in `sha256` (lowercase hex of the file) so the app can verify the download.
- `minAppVersion` is the app versionCode; `priority` picks among several models.
