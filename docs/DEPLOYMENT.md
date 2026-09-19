# Deployment

## Production

- GitHub: `https://github.com/strobofactory/pkpassport-for-mac`
- Branch: `main`
- Vercel project: `pkpassport-for-mac`
- Production URL: `https://pkpassport-for-mac.vercel.app/`
- Framework preset: Other
- Build command: none
- Root directory: repository root

## Release flow

1. Synchronize the local `main` branch with `origin/main`.
2. Serve the repository root locally over HTTP.
3. Verify the desktop and approximately `390px` layouts, required sections, interactive controls, and browser console.
4. Commit the verified static files and push `main` to GitHub.
5. Wait for the Git-connected Vercel production deployment to reach `READY`.
6. Confirm that the production alias serves the pushed commit without missing local assets.

## Local preview

From the repository root:

```sh
python3 -m http.server 8000
```

Open `http://127.0.0.1:8000/`. No package installation or build step is required.

## Rollback

Revert the unwanted commit on `main` and push the revert. Vercel will publish the restored repository state through the same Git integration.
