# status.akn.me.uk

Status page for my services — monitors uptime across Halcyon, Startpage, Letters, EchelonAPI, EtonSTEM, aknWiki, and Pathway.

Powered by GitHub Actions: `health-check.sh` runs hourly, appends results to log files, and commits. The page is served on GitHub Pages at [status.akn.me.uk](https://status.akn.me.uk).

## Services monitored

| Service | URL |
|---------|-----|
| Halcyon | https://akn.me.uk |
| Iris | https://iris.akn.me.uk |
| Letters | https://letters.akn.me.uk |
| EchelonAPI | https://api.akn.me.uk |
| EtonSTEM | https://etonstem.com |
| aknWiki | https://docs.akn.me.uk |
| Pathway | https://tpi.akn.org.uk |

## Adding a service

Edit `urls.cfg`:

```
ServiceName=https://example.com
```

The health check picks up new entries on the next hourly run.
