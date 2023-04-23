# github-actions-create-pull-request-demo

[![Pull Request](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/pull-request.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/pull-request.yml)
[![Release](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/release.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/release.yml)

GitHub Actions pull request workflow:

- If there is at least 1 new commit to `master`, a release PR will be opened to `production`.
- If a PR to `master` is created while the release PR is still open, then the PR to `master` will be converted to a draft with a comment.
- If the release PR is merged, then any open PRs to `master` will be ready for review with a comment.

See the [workflow](.github/workflows/pull-request.yml).

> **Note**: For this to work, you must go to **Settings** > **Actions** > **General** > **Workflow permissions** and enable:
>
> - [ ] Read and write permissions
> - [ ] Allow GitHub Actions to create and approve pull requests

## License

[MIT](LICENSE)
