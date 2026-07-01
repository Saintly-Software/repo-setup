Add these commands to `package.json`:

- `typecheck` – verifies type correctness in the app, does not emit any files
- `fmt:check` – runs code formatter in "check" mode (does not do any write ops)
- `lint:check` – runs code linter in "check" mode (does not do any write ops)
- `fmt` – runs code formatter in "write" mode (auto-updates files)
- `lint` – runs code linter in "write" mode (auto-updates files)

Create a github actions workflow that runs on every PR push and every push (merge) to main. Call it "quality check". It should do: 

1. `fmt:check`
2. `lint:check`
3. `typecheck`