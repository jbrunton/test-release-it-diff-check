Small test case for [release-it #687](https://github.com/release-it/release-it/issues/687).

Run `npm release`.

Current behavior:

```
npm run release

> @ release /Users/jbrunton/git/test-release-it-diff-check
> release-it

✔ touch index.js
ERROR Working dir must be clean.
Please stage and commit your changes.
Alternatively, use `--no-git.requireCleanWorkingDir` to include the changes in the release commit (or save `"git.requireCleanWorkingDir": false` in the configuration).
```

After using npm link to run using the `improve-clean-repo-check` branch on [jbrunton/release-it](https://github.com/jbrunton/release-it), it should pass the git checks instead.
