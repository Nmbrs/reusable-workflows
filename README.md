<h1 align="center">Welcome to reusable-workflows👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg" />
  <a href="LICENSE.md" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg" />
  </a>
</p>

> Repository containing GitHub reusable workflows used at Nmbrs

## Creating a reusable workflow

For more information on how to create a reusable workflow, please see [github documentation](https://docs.github.com/en/enterprise-cloud@latest/actions/using-workflows/reusing-workflows#creating-a-reusable-workflow)

## Calling a reusable workflow

You can call reusable workflows by using the keyword `uses` and referencing them into your workflow. Here are some examples:

### Referencing a workflow using commit hash

```yaml
jobs:
  call-workflow-in-your-local-repository:
    uses: nmbrs/reusable-workflow/.github/workflows/workflow.yaml@3a6cdac4e4094ccae7f92a1229db08d0ce3dbd7f
```

### Referencing a workflow using branch name

```yaml
jobs:
  call-workflow-in-your-local-repository:
    uses: nmbrs/reusable-workflow/.github/workflows/workflow.yaml@main
```

### Referencing a workflow using tags

```yaml
jobs:
  call-workflow-in-your-local-repository:
    uses: nmbrs/reusable-workflow/.github/workflows/workflow.yaml@v1
```

## Contributing

We've set up a separate document for our [contribution guidelines](CONTRIBUTING.md).

## Release History

Please see [CHANGELOG.md](CHANGELOG.md).

## Author(s)

👤 **Nmbrs - Infra Squad**

## 📝 License

This project is [MIT](LICENSE.md) licensed.
