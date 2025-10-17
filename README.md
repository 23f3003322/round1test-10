# Markdown to HTML Demo (GitHub Pages)

A tiny static site that loads Markdown from an attached input.md file, converts it to HTML using marked, renders it inside the #markdown-output container, and applies code highlighting with highlight.js.

## Project Summary
- Static site ready for GitHub Pages.
- Reads input.md from attachments (simulated via a data URL in this project).
- Uses marked to convert Markdown to HTML.
- Uses highlight.js to format syntax-highlighted code blocks.
- Renders the resulting HTML inside the page DOM element with id="markdown-output".

## Setup & Deployment (GitHub Pages)
1. Create a new repository on GitHub (e.g., your-username/markdown-demo).
2. Add all project files from this folder and commit:
   - git add .
   - git commit -m "Initial commit for GitHub Pages site"
3. Push to GitHub:
   - git push origin main
4. In the repository settings, enable GitHub Pages:
   - Source: main branch, / (root) or /docs if you place files under docs
   - Save, and note the published URL (e.g., https://your-username.github.io/markdown-demo/)
5. Visit the published URL to verify the page renders.

Alternatively, you can configure Pages to serve from the docs/ folder if you prefer a docs-based layout.

## Usage
- Open the published page in a browser.
- The Markdown input is loaded from input.md (presented here as a data URL to keep the site self-contained).
- Markdown is converted to HTML and inserted into the DOM under #markdown-output.
- Code blocks are syntax-highlighted using highlight.js.

## How the Code Works
- index.html
  - Loads marked (for Markdown parsing) and highlight.js (for code highlighting) from CDNs.
  - Contains a placeholder element for the attachment input (data URL) to demonstrate loading from attachments.
  - Converts the loaded Markdown to HTML and injects it into #markdown-output.
- styles.css
  - Basic responsive styling for a clean, readable layout.
- README.md
  - Project overview and setup instructions.

## Key Files
- index.html: Main page that wires together Markdown parsing and code highlighting.
- styles.css: Page styling.
- README.md: Project information and setup instructions.

## License
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
