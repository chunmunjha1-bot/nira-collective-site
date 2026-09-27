# The NiRa Collective — Website

Corporate site for The NiRa Collective LLC, a New Jersey umbrella holding company
(publishing, marketing, e-commerce).

- **Live:** https://theniracollective.com
- **Hosting:** Vercel (production deploys on every push to `main` via GitHub Actions)

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds and
deploys to Vercel production. Required repository secrets
(Settings → Secrets and variables → Actions):

| Secret | Value source |
|---|---|
| `VERCEL_TOKEN` | Vercel → Account Settings → Tokens |
| `VERCEL_ORG_ID` | Vercel project settings (team/account ID) |
| `VERCEL_PROJECT_ID` | Vercel project settings |

## Local preview

Open `index.html` in a browser, or serve it:

```sh
python3 -m http.server -d . 8000
```
