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

## Software / Libraries

- ESP32-A2DP (Bluetooth audio + metadata)
- Nextion Editor (touchscreen UI)
- lyrics.ovh API (lyrics lookup)

## Status

🚧 In development — Phase 1 focused on core music playback and display.

## License

MIT