# template-mathematica

A template with some automation tool for version controlling Wolfram Mathematica Notebook

### Prerequisites

`wolframscript` installed and already in the path

### How it works

`filter-output` will clean up all the `Cell` object  with `Output` tag before commiting. This script will be called from the git filter process, sanitizing the notebook from its output before staging to avoid large data such as images.

`render-precommit` will render all staged notebooks into pdf and store it in `Rendered`. This action is hooked to the git pre-commit hook.

(Optional) add a cron job to add a regular commit.




