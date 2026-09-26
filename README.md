# Seeker Agent Connect landing page

The public landing page for **Seeker Agent Connect (SAC)**. It is a static site with no build step.

| File | Purpose |
| --- | --- |
| `index.html` | Standalone landing page |
| `sac-interactive-screen.html` | Interactive app screen, embedded in the hero's phone by `index.html` (keep it next to `index.html`) |
| `.github/workflows/pages.yml` | Deploys the repository root to GitHub Pages on every push to `main` |

## Links

- Documentation lives in [SeekerAgentConnect/docs](https://github.com/SeekerAgentConnect/docs) and is published at <https://seekeragentconnect.github.io/docs/getting-started>. The landing page links to pages there by absolute URL (`https://seekeragentconnect.github.io/docs/<slug>`); update them if the docs move or a slug changes.
- GitHub, releases, deploy presets, security, and licence links point at [SeekerAgentConnect/sac](https://github.com/SeekerAgentConnect/sac).

## Local preview

```sh
python3 -m http.server 8000   # then open http://localhost:8000/
```

Serve the folder over HTTP rather than opening `index.html` from disk, so the embedded `sac-interactive-screen.html` loads.

## Publication

Merge into `main`. The **Pages** workflow publishes the site (Settings → Pages → Source must be **GitHub Actions**).
