# github-replace-version
Sets the README.md version.

## Example

```yaml
name: Generate
jobs:
  generate:
    steps:        
      - name: 'Get Previous tag'
        id: semver
        uses: "cdotyab/github-next-version@main"
        with:
          message: "${{github.event.head_commit.message}}"
        env:
          GITHUB_TOKEN: "${{ github.token }}"
      - name: 'Set Previous Version'
        uses: "cdotyab/github-replace-version@main"
        with:
          version: ${{steps.semver.outputs.version}}        
```

version:
* 1.0.0 - raw version
* v1.0.0 - raw tag formatted version


```
https://github.com/cdotyone/github-replace-version?ref=v0.0.0
```
