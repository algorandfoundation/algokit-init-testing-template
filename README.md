# algokit-init-testing-template

This template repository is used as a copier template example to drive some of the automated tests for the `algokit init` command.

These files are turned into a Git Bundle and added to https://github.com/algorandfoundation/algokit-cli/blob/main/tests/init/copier-helloworld.bundle.

This Git bundle is then referenced from the tests. This allows those tests to run locally without needing network access to clone this repository (and also improves the speed of the test execution).

To generate the git bundle run the following command in a Git clone of this repository:

```
git bundle create copier-helloworld.bundle --all
```

Alternatively, if using VS Code you can run the `Generate Git bundle for AlgoKit tests` task.

If you want to quickly test the output of the template when executing via algokit you can run one of these tasks in VS Code:

* `Run template using algokit (no-prompts)`
* `Run template using algokit (template prompts)`
