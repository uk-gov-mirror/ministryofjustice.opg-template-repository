# {{APP_TITLE}}

### Major dependencies

- [Go](https://golang.org/) (1.26.x)
- [docker compose](https://docs.docker.com/compose/install/) (>= 2.26.0)

#### Installing dependencies locally:
(This is only necessary if running without docker)

- `npm install`
- `go mod download`

---

#### Local development
The application is available at `http://localhost:{{PORT}}{{URL_PREFIX}}/`.

To enable debugging and hot-reloading of Go files:

`make dev-up`

Hot-reloading for web assets (JS, CSS, etc.) is provided via an npm watch command.
