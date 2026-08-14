# Bacon Digital Labs — Website

Marketing site for Bacon Digital Labs LLC, currently selling the **Lead Flow
Reliability Sprint** to local, owner-led service businesses (HVAC contractors
first).

Static HTML/CSS/JS — no build step, no framework, no dependencies.

## Local preview

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Hosting

Deployed via GitHub Pages from the `main` branch (`/root`). No custom domain
is configured yet; point DNS at GitHub Pages when a domain is registered:

1. Add a `CNAME` file to the repo root containing the domain.
2. In the registrar's DNS, add either:
   - an `A` record set pointing the apex domain at GitHub Pages' IPs, or
   - a `CNAME` record pointing a `www` subdomain at `<org>.github.io`.
3. Set the custom domain in the repo's **Settings → Pages**, and enable
   "Enforce HTTPS" once DNS has propagated.

See GitHub's docs: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site

## Structure

```
index.html       Single-page site
css/styles.css    Styles (light/dark aware)
js/main.js        Mobile nav + footer year
```
