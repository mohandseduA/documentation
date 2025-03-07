---
title: npm-test
section: 1
description: Test a package
github_repo: npm/cli
github_branch: release/v8
github_path: docs/content/commands/npm-test.md
redirect_from:
  - /cli-commands/npm-test
  - /cli-commands/test
  - /cli-documentation/cli-commands/npm-test
  - /cli-documentation/cli-commands/test
  - /cli-documentation/commands/npm-test
  - /cli-documentation/commands/test
  - /cli-documentation/npm-test
  - /cli-documentation/test
  - /cli-documentation/v8/cli-commands/npm-test
  - /cli-documentation/v8/cli-commands/test
  - /cli-documentation/v8/commands/npm-test
  - /cli-documentation/v8/commands/test
  - /cli-documentation/v8/npm-test
  - /cli-documentation/v8/test
  - /cli/cli-commands/npm-test
  - /cli/cli-commands/test
  - /cli/commands/npm-test
  - /cli/commands/test
  - /cli/npm-test
  - /cli/test
  - /cli/v8/cli-commands/npm-test
  - /cli/v8/cli-commands/test
  - /cli/v8/commands/test
  - /cli/v8/npm-test
  - /cli/v8/test
  - /commands/npm-test
  - /commands/test
---

### Synopsis

<!-- AUTOGENERATED USAGE DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/commands/test.js -->

```bash
npm test [-- <args>]

aliases: tst, t
```

<!-- automatically generated, do not edit manually -->
<!-- see lib/commands/test.js -->

<!-- AUTOGENERATED USAGE DESCRIPTIONS END -->

### Description

This runs a predefined command specified in the `"test"` property of
a package's `"scripts"` object.

### Example

```json
{
  "scripts": {
    "test": "node test.js"
  }
}
```

```bash
npm test
> npm@x.x.x test
> node test.js

(test.js output would be here)
```

### Configuration

<!-- AUTOGENERATED CONFIG DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->
#### `ignore-scripts`

* Default: false
* Type: Boolean

If true, npm does not run scripts specified in package.json files.

Note that commands explicitly intended to run a particular script, such as
`npm start`, `npm stop`, `npm restart`, `npm test`, and `npm run-script`
will still run their intended script if `ignore-scripts` is set, but they
will *not* run any pre- or post-scripts.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

#### `script-shell`

* Default: '/bin/sh' on POSIX systems, 'cmd.exe' on Windows
* Type: null or String

The shell to use for scripts run with the `npm exec`, `npm run` and `npm
init <package-spec>` commands.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

<!-- AUTOGENERATED CONFIG DESCRIPTIONS END -->

### See Also

* [npm run-script](/cli/v8/commands/npm-run-script)
* [npm scripts](/cli/v8/using-npm/scripts)
* [npm start](/cli/v8/commands/npm-start)
* [npm restart](/cli/v8/commands/npm-restart)
* [npm stop](/cli/v8/commands/npm-stop)
