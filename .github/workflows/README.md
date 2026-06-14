# Reusable workflows de CalleMedio

Centralizan el CI común. Para usarlos desde cualquier repo del org:

```yaml
# .github/workflows/ci.yml
name: CI
on: [push, pull_request]
jobs:
  ci:
    uses: CalleMedio/.github/.github/workflows/reusable-dotnet-ci.yml@main
    with:
      solution: MiApp.sln       # o reusable-node-ci.yml para TS
```
