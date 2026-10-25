Install [actionlint](https://github.com/rhysd/actionlint) to lint the github actions workflows in `.github/workflows/`. Pin it to an exact version.

Add an `actionlint` command to `package.json` that runs it against all workflow files. It does not write any files.

Add an `actionlint` step to the "quality check" workflow.
