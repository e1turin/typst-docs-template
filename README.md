# Scientific Research Work for Software Architecture Modeling and Scoring

To compile article's PDF use Ninja:
```sh
ninja doc
```

Or manually execute command `typst compile src/main.typ document.pdf`.

Note about development workflow: [dev.md](./docs/dev.md)

## Git workflow

Use this repository as a template, create a working branch, and commit your Typst and supporting-file changes there. Push the branch to GitHub and open a pull request when the document is ready for review. After merging (or from any branch with the required permissions), go to **Actions → Build PDF → Run workflow** and provide:

- the Typst source document to compile;
- the output PDF filename; and
- the GitHub Release tag that should contain the PDF.

The workflow keeps the PDF as a workflow artifact and publishes it as an asset on the specified GitHub Release.

## Referencies

Uses template `@preview/modern-g7-32:0.2.0` for article document.

Uses template `@preview/innovative-skoltech-slides` for presentation slides document.
