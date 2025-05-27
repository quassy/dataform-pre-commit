# Pre-commit hook for Dataform

This repository contains a pre-commit hook that allows you to automate the formatting of SQL and JS code in your Dataform project before each commit. The hook uses the `dataform format` command to format SQLX and JS files.

It also includes a hook that runs `dataform compile` before each commit to ensure that your Dataform project compiles successfully.

Alternatively you can use the dry run hook to run `dataform run --dry-run` to ensure the project compiles successfully and produces valid, executable SQL.

### How to Use

```
- repo: https://github.com/devoteamgcloud/pre-commit-dataform
  rev: [Fill with latest release]
  hooks:
    - id: dataform_format
    - id: dataform_compile
    - id: dataform_dry_run
```
