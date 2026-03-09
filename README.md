# z/OS Quiz Application

This simple static React/Tailwind quiz lives entirely in a set of HTML/JSON files and can be deployed on GitHub Pages.

## Deployment Steps

1. Create a new GitHub repository ("QuizApp" or similar).
2. Add all files from this `quiz` folder (including `index.html`, `quiz.html`, the four JSON banks, and any other assets) to the repo.
3. Commit and push to `main` (or `master`).
4. In the repository settings, enable **GitHub Pages** and set the source to the `main` branch and root folder. GitHub will serve `index.html` automatically.

> **Important**: the application uses relative paths when fetching JSON (`fetch('cobol.json')` etc.), so ensure the JSON files are in the same directory as `index.html`.

5. Optionally add a `404.html` redirect to `index.html` if you want client-side routing compatibility.

No build step is required; the code uses CDN-hosted React, ReactDOM and Babel to run directly in the browser.

## Customization
- Rename `index.html` to `quiz.html` or vice versa depending on preference.
- To change the default GitHub Pages URL you can set a custom `CNAME` file.

Once set up, your quiz will be live at `https://<username>.github.io/<repo>`.
