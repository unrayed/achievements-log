# gh CLI cheatsheet

```bash
gh auth status                      # token scopes and active account
gh repo list --limit 50             # repos with visibility
gh pr list --state all --json number,title,state,mergedAt
gh pr create --base main --title T --body B
gh pr merge --merge --delete-branch
gh api repos/{owner}/{repo}/branches/{branch}/protection
```

Notes:
- `gh api user --jq .login` confirms identity.
- Achievements are not in the API; only the profile HTML carries badge links.
