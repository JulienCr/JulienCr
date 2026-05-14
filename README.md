# Julien Cruau

_Video Engineer · Comédien · Code tinkerer_

---

I build live streaming tools by day. At night I'm on stage —
and somewhere between the two, I write the code that bridges them.

## Why I code (off the clock)

My day job is large-scale live video — and, for the past two years, the LLMs we plug into it. Off the clock, I code mostly to **outfit my own hobbies** instead of bending under software designed for someone else. An impro Twitch channel deserves its own cameras, its own overlays, its own server.

What pulls me in is the **hardware ↔ software bridge**. An X-Touch fader changing an OBS scene. An iPhone turned into a zero-latency NDI camera. A Stream Deck watching a Claude Code session and surfacing its state. Wiring things that didn't talk to each other — that's the part I love.

Open-notebook mode: many projects in parallel, few clean v1.0s, the occasional fork of my own tools to try a different stack. Deliberate. It stays a hobby, not a roadmap.

## Avolo — a Twitch channel and everything I had to code around it

[@la_scene_avolo](https://www.twitch.tv/la_scene_avolo) is a French impro channel. Off-the-shelf tools didn't cover what I needed as actor-and-engineer, so I ended up writing my own:

- **[avolo-cam](https://github.com/JulienCr/avolo-cam)** — Multi-iPhone → OBS. Three modes (NDI / Flash / SRT), GPU zero-copy decode, Tauri controller. The fastest camera I've managed to build.
- **[obs-live-suite](https://github.com/JulienCr/obs-live-suite)** — Control room: real-time overlays, interactive quiz, dockview dashboard, presenter comms. A 26-tool MCP server to drive it from Claude.
- **[xtouch-gw](https://github.com/JulienCr/xtouch-gw)** — Behringer X-Touch gateway for Voicemeeter / QLC+ / OBS, with motorised faders. TS v2 in production, Rust port underway to drop under 20 ms end-to-end.
- **[rythmo-impro](https://github.com/JulienCr/rythmo-impro)** — Live dubbing reader (rythmo) for impro sessions. WhisperX transcription + pyannote diarisation in Docker, Next.js frontend.

A few more pieces of this stack — server, booking-contract generator, auto-framing camera, logo animation — live in private repos.

## Outside Avolo

- **[streamdeck-claude](https://github.com/JulienCr/streamdeck-claude)** — Elgato plugin that surfaces live Claude Code session state on the deck. Useful when you've got three running in parallel.
- **[Wolf Gang Paris](https://www.wolfgangparis.com/)** — I designed and built the full show-control stack for this immersive escape-game venue: lighting, sound, network, scene logic, player interactivity. The website is mine too — currently mid v2 rebuild on Next.js.

## Stack & playgrounds

- **Languages** — TypeScript · Rust · Python · Swift · C# · Bash · PowerShell · PHP
- **Video & streaming** — OBS · NDI · SRT · HLS/DASH · FFmpeg · WhisperX · Remotion
- **Hardware & MIDI** — Behringer X-Touch · Stream Deck · Voicemeeter · QLC+
- **Infra & ops** — Ansible · YunoHost · Terraform · k6 · Home Assistant
- **AI & agents** — Claude Code · MCP · ONNX · CUDA · pyannote
- **Web** — Next.js · Astro · Tauri · Tailwind · PrestaShop

## Elsewhere

[avolo.fr](https://avolo.fr) · [twitch.tv/la_scene_avolo](https://www.twitch.tv/la_scene_avolo)

---

> _Profile tinkered together — like most of the rest._
