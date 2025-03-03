# Contributing to SciCat Projects

Each SciCat repository should have designated Maintainers (listed in the repository's MAINTAINERS.md file). They determine the repository's process for accepting contributions, articulated in the repository's CONTRIBUTING.md file.

Broadly, repositories should use one of the following workflows:

## Latest Stable
* Every change should go through a Pull Request.
* The person submitting a Pull Request should not merge their own Pull Request.
* Proposed changes with a large impact---including changes that introduce
  new concepts, technologies or depenencies; alter the project's scope; or make significant backward-incompatible changes---should be left open for at least one week to allow time for comment, and review should be solicited from a broad range of Maintainers or Contributors who may have useful input on the impact of the change. It is up to a repositiory's Maintainers to judge how much review is needed for a given Pull Request.
* This code should be in the `main` or `master` branch
* utilize automated CI pipelines to test prior PR merging

## Releases
* have releases with a clear naming convention. We suggest using semantic naming. 
* produce releases in a predictable manner and according to a schedule, if possbile.
* have a dedicated release branch
* utilize automated CI pipelines to test and versioning

## Experimental
SciCat projects are typically public from the very first commit. In this
early stage, the Maintainers have complete discretion about what
if any review is needed. Changes may be pushed directly to the `main`
branch; pull request may be self-merged.

## Non-code repositories
Non-code repositories should select a workflow repository-by-repository basis that matches the intended usage.


---
Licensed under the [CC-BY 4.0](https://creativecommons.org/licenses/by-sa/4.0/) License.
