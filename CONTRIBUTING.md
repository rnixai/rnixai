# rnixai Profile Repo

This repository is **only** for the [GitHub profile Overview](https://github.com/rnixai). The content of **README.md** is displayed there.

## Logo & avatar

- **`assets/icon.svg`** — Used in the profile README (top of page).
- **`assets/avatar.png`** (512×512) — Use as the **GitHub profile avatar**: [GitHub → Settings → Profile](https://github.com/settings/profile) → upload `avatar.png` (or download from [raw](https://raw.githubusercontent.com/rnixai/rnixai/main/assets/avatar.png)).

## Profile settings (Public profile)

Fill these at **[github.com/settings/profile](https://github.com/settings/profile)** (while logged in as **rnixai**):

| Field | Value |
|-------|--------|
| **Profile picture** | Upload `assets/avatar.png` (or [raw link](https://raw.githubusercontent.com/rnixai/rnixai/main/assets/avatar.png)) |
| **Name** | Rnix |
| **Bio** | An operating system for AI agents — Unix philosophy: process, VFS, syscalls. https://rnix.ai |
| **URL** (website) | https://rnix.ai |
| **Company** | Rnix |
| **Location** | _(optional)_ |
| **X (Twitter)** | _(optional)_ |

To update via CLI (requires `user` scope):  
`gh auth refresh -h github.com -s user` then:

```bash
gh api -X PATCH /user \
  -f name="Rnix" \
  -f bio="An operating system for AI agents — Unix philosophy: process, VFS, syscalls. https://rnix.ai" \
  -f blog="https://rnix.ai" \
  -f company="Rnix"
```

## Updating the profile

1. Edit **README.md** in this repo.
2. Commit and push:

   ```bash
   git add README.md
   git commit -m "docs: update profile overview"
   git push
   ```

3. Refresh https://github.com/rnixai to see the change.

No need to maintain this content in the rnix repo — this repo is the single source of truth.
