# hello-world

Blog and documentation site powered by MkDocs and Material for MkDocs.

## What this gives you

- Write articles as Markdown files.
- Automatically publish to GitHub Pages from the master branch.
- Keep docs and blog-like posts in one structure.

## Project structure

- docs/
  - index.md
  - articles/
	 - welcome.md
	 - writing-your-next-post.md
- mkdocs.yml
- requirements.txt
- .github/workflows/deploy.yml

## Local development

1. Install dependencies:

	pip install -r requirements.txt

2. Start the local docs server:

	mkdocs serve

3. Open the local URL shown in the terminal (usually http://127.0.0.1:8000).

## Add a new article

1. Create a new Markdown file inside docs/articles/.
2. Add it to nav in mkdocs.yml.
3. Commit and push to master.

The GitHub Actions workflow deploys the site automatically to GitHub Pages.

## First-time GitHub Pages setup

In your repository settings:

1. Open Pages.
2. Set Source to GitHub Actions.

After that, each push to master publishes the latest docs site.
