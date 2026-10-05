# Red Legacy Archive

This directory preserves the GitHub-native history that GitHub removes when a
fork leaves its fork network. The repository's complete Git history remains in
normal branches and tags; this archive supplements it with pull-request and
repository metadata.

## Recovery anchors

- Final legacy `main`: `d4fc2a9fcf0a7a43c4f0d0b0aecb6631397bdd49`
- Open CTF research PR #26 head: `e392f1ae791b28b521296eb900a1b1bd8c79f247`
- Original evidence-led workflow commit: `cad6a525c59a46d87295f2b5ee73a3b109faeefb`
- Fullpwn documentation commit: `e392f1ae791b28b521296eb900a1b1bd8c79f247`

## Contents

- `github-export/`: repository settings plus all 26 pull requests, including
  bodies, comments, reviews, review comments, timelines, commits, files, diffs,
  and patches.
- `git-refs.txt`: branch, tag, and pull-request refs captured before detachment.
- `github-export/SHA256SUMS`: integrity manifest for every exported artifact.

The local Conductor workspace also retains a verified mirror repository and a
portable Git bundle under `.context/backups/`; those backups are intentionally
not committed to GitHub.
