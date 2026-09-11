# Echo-Inspired Smart Bluetooth Speaker

A DIY smart Bluetooth speaker built on the ESP32, featuring a Nextion touchscreen that displays now-playing song info, playback controls, incoming call notifications, and more — inspired by the Amazon Echo.

## Features

- Bluetooth A2DP music streaming with song title, artist, and progress bar
- Playback controls: play, pause, skip, shuffle, and loop
- Live clock and connected device name shown on screen
- Incoming call notifications with a drop-down banner and answer/decline buttons
- Automatic music ducking during calls
- On-screen volume control
- Lyrics lookup (stretch feature)

## Hardware

- ESP32 dev board
- Nextion touchscreen (5")
- I2S DAC (e.g. PCM5102A)
- Amplifier (e.g. PAM8403)
- Speaker driver
- 5V power supply / external battery
- Battery management chip (e.g. MAX17048) — for battery % readout

## Software / Libraries

- ESP32-A2DP (Bluetooth audio + metadata)
- Nextion Editor (touchscreen UI)
- ESP-IDF HFP client API (call handling)
- lyrics.ovh API (lyrics lookup)

## Roadmap

### Phase 1 — Core Build
- ESP32 ↔ phone Bluetooth (A2DP) connection
- Now-playing screen: song title, artist, progress bar
- Playback controls: play, pause, skip, shuffle, loop
- Live clock (corner of screen)
- Connected device name shown on screen
- Connection chime when a device pairs
- Wi-Fi and battery status icons

### Phase 2 — Call Handling
- HFP integration for caller ID and call state
- Dynamic-island style drop-down banner on incoming calls
- Answer/decline buttons on the banner
- Automatic music ducking during calls
- Dedicated call screen: caller name, live call duration, volume control, end call
- Decline from banner resumes music immediately, no call screen shown
- Standalone on-screen volume button (independent of calls)

### Phase 3 — Stretch Goals
- Lyrics page via lyrics.ovh API (WiFi-based lookup)
- Album cover art via AVRCP 1.6 / Bluetooth Image Profile

## Status

🚧 In development — Phase 1 focused on core music playback and display.

## License

MIT