# Thoughts, Unfolded

A gentle browser-based space to reflect on thoughts and choose a next step.

## Privacy and model loading

Emotion signals are calculated in the browser. Writing is not sent to an inference API and is not saved automatically. The page downloads its JavaScript runtime and model assets from jsDelivr and Hugging Face, so the first visit needs an internet connection and may take a little longer while the model loads.

## GitHub Pages

The workflow in `.github/workflows/deploy-pages.yml` packages `thoughts-unfolded.html` as the site’s `index.html` and deploys on pushes to `main` or a manual workflow run. In the repository’s **Settings → Pages**, choose **GitHub Actions** as the build and deployment source.