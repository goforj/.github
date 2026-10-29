<p align="center">
  <a href="https://goforj.dev">
    <img src="https://raw.githubusercontent.com/goforj/docs/e63d7a15a5c6e4d7b4a2b930d10913433d90da33/docs/public/twitter-banner.png" width="100%" alt="GoForj: The composable stack for building with Go, illustrated by the Foundry workbench">
  </a>
</p>

<p align="center">
  <strong>Go tools forged for speed, clarity, and confidence.</strong>
</p>

<p align="center">
  <a href="https://goforj.dev">Documentation</a> ·
  <a href="https://github.com/goforj/goforj">Application toolkit</a> ·
  <a href="https://github.com/orgs/goforj/repositories">All projects</a>
</p>

GoForj is a composable stack for building Go applications, with focused libraries for everyday code, HTTP, background work, and infrastructure. The `forj` CLI brings them together in generated projects with explicit wiring and app-owned source.

Use the standalone libraries in an existing Go application, or [start a GoForj project](https://goforj.dev/getting-started/quickstart) to build APIs, workers, scheduled jobs, command-line tools, and web apps.

## Standalone libraries

### Everyday Go

| Library | What it helps you build |
| ---: | --- |
| [collection](https://github.com/goforj/collection) | Typed, fluent slice pipelines for mapping, filtering, sorting, grouping, and reducing. |
| [str](https://github.com/goforj/str) | Immutable string transformations, Unicode-aware helpers, matching, and inflection. |
| [env](https://github.com/goforj/env) | Typed environment configuration with dotenv loading, scoped keys, fallbacks, and required-value checks. |
| [crypt](https://github.com/goforj/crypt) | Authenticated encryption for application payloads, with key rotation and compatibility with earlier payload formats. |
| [godump](https://github.com/goforj/godump) | Readable dumps and diffs of Go values, with terminal and HTML output, cycle handling, and field redaction. |

### HTTP and CLI applications

| Library | What it helps you build |
| ---: | --- |
| [web](https://github.com/goforj/web) | HTTP handlers, routing, middleware, WebSockets, and handler tests through focused contracts and an Echo adapter. |
| [httpx](https://github.com/goforj/httpx) | Fluent HTTP clients with typed responses, authentication, retries, and request diagnostics, built on `req`. |
| [console](https://github.com/goforj/console) | CLI output with semantic messages, tables, trees, interactive prompts, loaders, and progress indicators. |
| [execx](https://github.com/goforj/execx) | Subprocess workflows with explicit arguments, streaming output, typed decoding, and TTY support. |
| [metrics](https://github.com/goforj/metrics) | Application instrumentation with counters, gauges, histograms, snapshots, and Prometheus text output, using only the standard library. |

### Background work and infrastructure

| Library | What it helps you build |
| ---: | --- |
| [queue](https://github.com/goforj/queue) | Background jobs with pluggable backends, workers, retries, delayed jobs, uniqueness, chains, and batches. |
| [events](https://github.com/goforj/events) | Typed event publication and fan-out, in-process or through distributed pub/sub drivers such as NATS, Redis, Kafka, and Google Pub/Sub. |
| [scheduler](https://github.com/goforj/scheduler) | Fluent cron, interval, and calendar schedules with filters, lifecycle hooks, and overlap protection. |
| [cache](https://github.com/goforj/cache) | Local, distributed, and SQL-backed caching with typed helpers, locks, counters, and rate limits. |
| [storage](https://github.com/goforj/storage) | One file-storage API for local disks, S3, Google Cloud Storage, Redis, SFTP, FTP, and rclone remotes. |
| [mail](https://github.com/goforj/mail) | Fluent email composition with delivery drivers for SMTP, SES, Resend, Postmark, Mailgun, and SendGrid. |

## Application and developer tooling

| Project | What it provides |
| ---: | --- |
| [goforj](https://github.com/goforj/goforj) | The application stack and `forj` CLI: project creation, component wiring, Vue/React/templ + htmx starters, and a local development workflow. |
| [wire](https://github.com/goforj/wire) | Compile-time dependency injection with generation caching, watch mode, and `go tool` support. Maintained fork of Google Wire, usable in any Go project. |
| [atlas](https://github.com/goforj/atlas) | Project guidance, skills, and MCP tools that help coding agents inspect and navigate GoForj applications. |

## How we build

- **Explicit by default.** Configuration and behavior stay visible and auditable.
- **Composable by design.** Small packages expose narrow APIs and avoid unnecessary coupling.
- **Confidence through tests.** Core behavior, failure paths, and integrations are exercised in CI.
- **Performance with evidence.** Benchmarks guide decisions where speed or allocation behavior matters.

## Project status

**The GoForj framework is in public beta.** Start building Go applications, explore the independently versioned libraries, and help shape the framework before 1.0.

[Get started](https://goforj.dev/getting-started/quickstart) · [Release status](https://goforj.dev/versions/#public-beta)

Open an issue on the relevant project to share feedback.

## Contributing

Bug reports, documentation improvements, benchmarks, focused fixes, and design discussions are welcome. Please use the issue tracker for the project your contribution affects.

## License

GoForj projects are released under the MIT license unless a repository states otherwise.
