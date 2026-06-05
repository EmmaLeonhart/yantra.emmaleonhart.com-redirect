# yantra.emmaleonhart.com redirect

Static GitHub Pages site that redirects **yantra.emmaleonhart.com** → <https://yantraos.org/>.

`yantra.emmaleonhart.com` is the legacy subdomain for the Yantra project, which now
lives on its own domain `yantraos.org`. This repo forwards all traffic (preserving
path, query string, and hash) to the new domain. GitHub Pages issues a free
Let's Encrypt certificate for the custom domain so `https://yantra.emmaleonhart.com`
keeps a valid TLS certificate.

## DNS setup (to do at the registrar)
Point `yantra.emmaleonhart.com` at GitHub Pages with a CNAME record:
- `yantra.emmaleonhart.com` → `emmaleonhart.github.io` (or the appropriate Pages host)

The `CNAME` file in this repo sets the Pages custom domain to `yantra.emmaleonhart.com`.
