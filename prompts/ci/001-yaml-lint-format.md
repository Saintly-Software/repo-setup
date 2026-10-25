Add a YAML linter and formatter, and apply them to every `.yml` / `.yaml` file in the project (including `.github/`).

- Lint with [yamllint](https://github.com/adrienverge/yamllint). Pin it to an exact version.
- Format with `oxfmt`, which supports YAML. If `oxfmt` is not installed, use [yamlfmt](https://github.com/google/yamlfmt) instead.

Make sure the linter and formatter agree with each other (indentation, line length, quoting), so one never undoes the other.

Add the YAML files to the existing `fmt:check` / `fmt` commands. Add a `yaml:lint` command to `package.json` that runs the linter in "check" mode (does not do any write ops).

Add `yaml:lint` to the "quality check" workflow.
