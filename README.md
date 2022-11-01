# Public Workflows

**This repository is intentionally public.** Use it with caution.

Store loft-br reusable workflows here. Check GitHub documentation for this feature: [Reusable Workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows).

## Use Cases

Check [the documentation](https://docs.github.com/en/actions/using-workflows/reusing-workflows) for more information on reusable workflows.

### For workflows maintainers

Use this repository to store large workflows intended for reuse inside [loft-br](https://github.com/loft-br). The files will be publicly available, therefore should be revised before commited to the repo.

### For workflows consumers

Call a reusable workflow from your repository with the `uses` keyword at the job level. Check the syntax to use the `loft-br/public-workflows` repository's `my-reusable-workflow.yaml`:

```yaml
# .github/workflows/your-workflow-in-your-repository.yml
on:
  some_event:
jobs:
  callReusableWorkflow:
    uses: loft-br/public-workflows/.github/workflows/my-reusable-workflow.yaml@main
```

## License

All files stored here are licensed under [The Unlicensed](https://github.com/loft-br/public-workflows/blob/main/LICENSE). Therefore, you shouldn't store here anything that can't be copied, modified, published, used even or sold by someone else.
