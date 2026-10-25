# Documentation project instructions

## About this project

- Public documentation for the bapsolver API at `https://api.bapsolver.xyz`, built on [Mintlify](https://mintlify.com).
- Pages are MDX files with YAML frontmatter. Configuration lives in `docs.json`.
- Endpoint pages are generated from `openapi.json`. Change the endpoint text there, not in MDX.

## Content boundaries

- Document only what an API caller needs: authentication, endpoints, job fields, results, errors and limits.
- Do not document how tokens are made: the execution environment, device profiles, TLS or HTTP/2 fingerprints, recipes, the worker or deployment.
- Do not document the internal `/v1/status` route.
- Use synthetic examples only: `www.example.com`, `YOUR_SITE_KEY`, documentation IP ranges such as `203.0.113.0/24`. Never paste a real token, site key, proxy or API token.

## Terminology

- "API token" for the bearer credential; "token" or "reCAPTCHA token" for the job result.
- "job", "job kind", "site key", "action".

## Style preferences

- Use active voice and second person ("you").
- Keep sentences short, one idea per sentence.
- Use sentence case for headings.
- Use code formatting for fields, codes, headers, paths and commands.
- Keep each subject on one page and link to it instead of repeating it.
