# DOOM.DOC

A symptom-checker parody: select symptoms, get an absurd diagnosis, and copy the result to share. Built with plain HTML, CSS, and JavaScript in a single file.

**Entertainment only. The diagnoses are fictional and are not medical advice.**

## Run locally

Open `index.html` in your browser. No installation, build step, API keys, or backend is required.

For a local server, run the following from the project folder, then visit <http://localhost:8000>:

```sh
python -m http.server 8000
```

Clipboard access works best on localhost or HTTPS.

## Development

Edit `index.html`, which contains the page markup, styles, symptom data, and application logic.

Optional formatting tools require Node.js and npm:

```sh
npm ci
npm run format
npm run check
```

Formatting is checked automatically on pushes and pull requests to `main`.

## Repository layout

- `index.html`: the complete app and static hosting entry point.
- `.github/workflows/check.yml`: formatting check.
- `.editorconfig`, `.gitattributes`, and `.prettierrc.json`: consistent formatting and line endings.
- `.gitignore`: excludes credentials, generated files, and local exports.

The original duplicate exports are retained locally in the ignored `.local-originals/` directory. Make future changes in `index.html`.

## Contributing

Keep changes focused, preserve the satire disclaimer, run `npm run check`, and describe the behavior you changed in your pull request. For UI changes, check both a narrow mobile viewport and a desktop browser.
