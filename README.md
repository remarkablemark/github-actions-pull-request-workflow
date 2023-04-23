# github-actions-pull-request-workflow

[![Create Pull Request](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/create-pull-request.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/create-pull-request.yml)
[![Check Merge](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/check-merge.yml/badge.svg)](https://github.com/remarkablemark/github-actions-pull-request-workflow/actions/workflows/check-merge.yml)

GitHub Actions pull request workflow:

- If there's a commit to `master`, then a release PR will be opened to `production`. Open PRs will be converted to draft.
- If a PR to `master` is created while a release PR is open, then the PR to `master` will be converted to draft.
- If the release PR is merged, then any open PRs to `master` will be converted from draft to ready for review.

> **Note**: For this to work, you must go to **Settings** > **Actions** > **General** > **Workflow permissions** and enable:
>
> - [ ] Read and write permissions
> - [ ] Allow GitHub Actions to create and approve pull requests

## License

[MIT](LICENSE)
