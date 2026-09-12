# Scientific Research Work for Software Architecture Modeling and Scoring

To compile article's PDF use Ninja:
```sh
ninja article
```

Or manually execute command `typst compile src/main.typ article.pdf`.

Note about development workflow: [dev.md](./misc/dev.md)

## Git workflow

Use this repository as a template, create a working branch, and commit your Typst and supporting-file changes there. Push the branch to GitHub and open a pull request when the document is ready for review. After merging (or from any branch with the required permissions), go to **Actions → Build PDF → Run workflow** and provide:

- the Typst source document to compile;
- the output PDF filename; and
- the GitHub Release tag that should contain the PDF.

The workflow keeps the PDF as a workflow artifact and publishes it as an asset on the specified GitHub Release.
