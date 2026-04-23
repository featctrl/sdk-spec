# Changelog

All notable changes to the featctrl SDK specifications are documented here.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [0.1.0] – 2026-04-23

### Added
- Initial specification covering the full SSE connection lifecycle.
- Data model: `Flag` (boolean type).
- Endpoints: `GET /sse`, `POST /heartbeat`, `DELETE /disconnect`.
- SSE events: `connection.established`, `flags.snapshot`, `flag.changed`, `flag.deleted`, `heartbeat`, `reconnect`.
- Implementation constraints: flag cache, connection modes (`livestreaming`, `snapshot`), reconnection procedure, heartbeat watchdog, degraded mode, environment variables.
