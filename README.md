# github-actions-create-pull-request-demo

[![Pull Request](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/pull-request.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/pull-request.yml)
[![Release](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/release.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/release.yml)

GitHub Actions pull request workflow:

- If there's at least 1 commit to `master`, a release PR will be opened to `production`.
- If a PR to `master` is created while a release PR is open, then the PR to `master` will be converted to a draft.
- If a release PR is merged, then any open (draft) PRs to `master` will be ready for review.

See the [workflow](.github/workflows/pull-request.yml).

> **Note**: For this to work, you must go to **Settings** > **Actions** > **General** > **Workflow permissions** and enable:
>
> - [ ] Read and write permissions
> - [ ] Allow GitHub Actions to create and approve pull requests

## License

[MIT](LICENSE)
