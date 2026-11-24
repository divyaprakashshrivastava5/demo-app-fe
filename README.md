# demo-app-fe

Static frontend for DeployPanel multi-service dogfood (from `examples/multiservice/web`).

## DeployPanel deploy

| Setting | Value |
|---------|-------|
| Language | `static` (nginx serves `index.html`) |
| Container listen | port **80** |
| Typical host publish | **8080** (wizard maps host → container 80) |
| Env | none required |
| Dockerfile | not required — DeployPanel generates one |

Pair with the API repo [demo-app-be](https://github.com/divyaprakashshrivastava5/demo-app-be) and optional Postgres. The page calls `{hostname}:3001/api/hello` by default (override with `window.API_BASE`).

## Local preview

Open `index.html` in a browser, or serve the folder with any static file server.
