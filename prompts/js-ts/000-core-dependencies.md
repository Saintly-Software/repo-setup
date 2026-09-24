Use node v26 and pnpm v11. (Make sure to specify minor + patch versions.) Initialize the project with these tools if not already done.

Replace `npm` with `pnpm` if not already done.

Set an `.nvmrc` for the node version if not already done.

Add the following dev dependencies:

- typescript v6
- oxlint
- oxfmt
- changeset

Initialize each of these dependencies appropriately. You should see config files (or something like that) for each of them.

For oxlint and oxfmt, prefer TypeScript config files (`oxlint.config.ts`, `oxfmt.config.ts`) over JSON config files (`.oxlintrc.json`, `.oxfmtrc.json`). If JSON config files already exist, migrate them to `.ts` and delete the JSON versions.

Ensure `.gitignore` is set up correctly (ignores node_modules, etc.).

Set `pnpm` as the `packageManager` in  `package.json` if not already done.

Set the "engine" attribute in package.json to be in sync with the node version.
