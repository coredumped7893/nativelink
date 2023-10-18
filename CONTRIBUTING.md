# Contributing to Turbo Cache

Turbo Cache welcomes contribution from everyone. Here are the guidelines if you
are thinking of helping us:

## Contributions

Contributions to Turbo Cache or its dependencies should be made in the form of
GitHub pull requests. Each pull request will be reviewed by a core contributor
(someone with permission to land patches) and either landed in the main tree or
given feedback for changes that would be required. All contributions should
follow this format, even those from core contributors.

Should you wish to work on an issue, please claim it first by commenting on
the GitHub issue that you want to work on it. This is to prevent duplicated
efforts from contributors on the same issue.

## Pull Request Checklist

- Branch from the main branch and, if needed, rebase to the current main
  branch before submitting your pull request. If it doesn't merge cleanly with
  main you may be asked to rebase your changes.

- Commits should be as small as possible, while ensuring that each commit is
  correct independently (i.e., each commit should compile and pass tests).

- Commits should be accompanied by a [Developer Certificate of Origin](http://developercertificate.org)
  sign-off, which indicates that you (and your employer if applicable) agree to
  be bound by the terms of the [project license](LICENSE). In git, this is the
  `-s` option to `git commit`.

- If your patch is not getting reviewed or you need a specific person to review
  it, you can @-reply a reviewer asking for a review in the pull request or a
  comment.

- Add tests relevant to the fixed bug or new feature.

- If `rustfmt` complains you can use the following command to apply its
  suggested changes to the Rust sources:

  ```bash
  bazel run \
    --@rules_rust//:rustfmt.toml=//:.rustfmt.toml \
    @rules_rust//:rustfmt
  ```

## Conduct

Turbo Cache Code of Conduct is available in the
[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) file.