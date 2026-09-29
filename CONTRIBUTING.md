# Contribution guide

Thank you for contributing to this repository! To keep collaboration smooth, please follow the rules below.

## How to Contribute

1. Before making changes, create an Issue or check for an existing one.
2. Fork the repository and create a working branch.
3. Commit your changes and open a Pull Request (PR).
4. Once reviewed and approved, your PR will be merged.

## Commit Message Rules

Every commit message **MUST** follow this format:

```
fix: #XXX, <message>
```

- `#XXX` is the issue number linked to your work. Every commit must reference exactly one issue.
- The commit message must be meaningful, clearly describing what has changed.
- Vague messages such as `WIP`, `update`, `fix stuff`, or `asdf` are not allowed.

### Good examples

```
fix: #12, correct the broken quadratic formula notation
fix: #7, update the reference URL that had a dead link
```

### Bad examples

```
update
update notes
fix: correct typo        (missing issue number)
fix: #3, fix              (meaningless description)
```

## Pull Request Rules

- Each PR must contain exactly one commit.
    - If you ended up with multiple commits during your work, squash them into one before merging.
    - Use `git rebase -i` or `git commit --amend` to tidy up your commits.
- The PR title must also follow the `fix: #XXX, <description>` format, matching the commit message.
- Reference the related issue in the PR body as `Closes #XXX` so the issue is closed automatically on merge.

### How to squash into a single commit

```bash
# Clean up the last N commits
git rebase -i HEAD~N

# Or append changes to the last commit
git add .
git commit --amend
```
