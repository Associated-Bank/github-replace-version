# Semantic Versioning Prefix Table
Here’s a list of allowed prefixes and their respective semantic version (SemVer) increment type:

| Prefix | SemVer Increment | Description| 
|--------|------------------|------------|
| feat | Minor | A new feature |
| fix | Patch | A bug fix |
| docs | None | Documentation only changes |
| style | None | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc) |
| refactor | None | A code change that neither fixes a bug nor adds a feature |
| perf | Patch | A code change that improves performance |
| test | None | Adding missing tests or correcting existing tests |
| build | None | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm) |
| ci | None | Stands for Continuous Integrations. Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |
| chore | None | Other changes that don't modify src or test files |
| revert | None | Reverts a previous commit |

# Example Usage During Commit
git commit -m "docs: updating documentation" <br />
git commit -m "build: adding semantic-release" <br />