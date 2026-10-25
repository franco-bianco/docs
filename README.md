# bapsolver API docs

Source for the public bapsolver API documentation, built with [Mintlify](https://mintlify.com).

## Layout

| Path                    | Holds                                                     |
| ----------------------- | --------------------------------------------------------- |
| `docs.json`             | Site settings and navigation                              |
| `index.mdx`, `quickstart.mdx`, `authentication.mdx` | Get started                   |
| `concepts/`             | Jobs, job kinds and proxies, using tokens                 |
| `reference/`            | Errors and limits                                         |
| `api-reference/`        | API overview; endpoint pages come from `openapi.json`     |
| `openapi.json`          | The public OpenAPI document                               |

## Preview

```sh
npm i -g mint
mint dev
```

Open `http://localhost:3000`. Run `mint broken-links` before you push.

## Publish

A push to `main` deploys the site through the Mintlify GitHub app.

## Update the API reference

`openapi.json` comes from the API's own OpenAPI document (`src/api/openapi.ts` in the API repository), with the internal `/v1/status` and `/openapi.json` routes removed and the production server set. When the API changes, regenerate it and update the guide pages that describe the change.
