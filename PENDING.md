# PENDING.md — novus-aeyre (Æyre)

Durable cross-session backlog. Not rewritten each session — items persist until resolved or explicitly dropped.

- **Voice scaffold works via `--demo` only** — live mic loop not yet verified.
- **Vision not started** — no code, no design beyond stub directories.
- **Voice engine still lives in `aesop-xi/voice-engine/`** (temporary) — needs extracting into `app/audio/`, `app/vad/`, `app/stt/`, `app/tts/` per the planned layout in `README.md`, then wiped from `aesop-xi`.

## Carried over from unresolved.md (2026-10-08)


- **Live mic loop not verified.** Only `--demo` has been run end-to-end.
  Don't build further on the mic path until this is confirmed working.
- **Vision path has no design.** Camera capture + LiteHRNet inference,
  zero code, zero spec beyond the `screen-vision/` stub directory. No
  raw source material was retrievable this session to seed it (see
  `RESUME.md` — the relevant Drive subfolder isn't shared with this session
  and its content was already synthesized into `novaexopia`, not this repo).
- **HTTP/WebSocket server for remote voice-engine invocation** — spec'd in
  `aesop-xi/ARCHITECTURE.md` (Flask/FastAPI wrapping `VoiceEngine`),
  deliberately deferred, never built. See `novae-xorpus/unresolved.md` item 7.
- **Voice engine extraction from `aesop-xi/voice-engine/` not yet done** —
  currently lives there temporarily under Termux + Debian proot; the plan is
  to move it here and wipe it from `aesop-xi`, not yet executed.
