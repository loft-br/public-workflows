# Public Workflows

**This repository is intentionally public.** Use it with caution.

Store loft-br reusable workflows. Check GitHub documentation for this feature: [Reusable Workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows).

## Use Cases

Check [the documentation](https://docs.github.com/en/actions/using-workflows/reusing-workflows) for more information on reusable workflows.

### For workflows maintainers

Use this repository to store large workflows intended for reuse inside [loft-br](https://github.com/loft-br). The files will be available to the public, therefore should be revised before commited to the repo.

### For workflows consumers

Call a reusable workflow from your repository by using the `uses` keyword in your workflow file. For example, to use the `loft-br/reusable-workflows` repository's `main.yml` workflow file, use the following syntax:

```yaml
# .github/workflows/your-workflow-in-your-repository.yml
on:
  some_event:
jobs:
  callReusableWorkflow:
    uses: loft-br/public-workflows/.github/workflows/my-reusable-workflow.yaml@main
```

## License

All files stored here is licensed under [The Unlicensed](https://github.com/loft-br/public-workflows/blob/main/LICENSE), therefore don't store your workflow here if there is any trouble in it being copied, modified, published, used, etc.
