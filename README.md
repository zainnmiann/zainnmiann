# Muhammad Zain Mian

**Embedded systems and IoT.** I build systems where hardware, firmware and software meet:
indoor positioning with ultra-wideband radios, weather stations that report over LoRa,
and computer vision on edge GPUs. I like work I can test on a bench and then deploy in the field.

```mermaid
flowchart LR
    S["Sensors & UWB radios"] --> F["Firmware<br/>C · nRF52 · ESP32"]
    F --> R["Radio link<br/>UWB · LoRa · cellular"]
    R --> E["Edge<br/>Raspberry Pi · Jetson"]
    E --> M(("MQTT"))
    M --> B["Backend & models<br/>Python · Postgres · Docker"]
```

### Currently

- Improving UWB ranging accuracy: antenna-delay calibration, per-anchor bias maps and first-path (CIR) detection in multipath
- Building rain and wind forecasts for a single hyperlocal weather station

### Featured

| Project | What it does | Built with |
|---|---|---|
| [**uwb_tdma_twr**](https://github.com/zainnmiann/uwb_tdma_twr) | One UWB ranging firmware for two platforms. Any DWM1001 or ESP32 board can be a tag or an anchor in the same TDMA DS-TWR network, verified on hardware | C · nRF52832 · ESP32 · DW1000 |
| [**dwm1001-uwb-dstwr-firmware**](https://github.com/zainnmiann/dwm1001-uwb-dstwr-firmware) | RTLS firmware for DWM1001-DEV: initiator-driven fixed-slot DS-TWR, up to 12 anchors and 32 tags, ~7.2 Hz per tag measured on a 10 × 9 schedule, plus host simulator and Pi bridge | C · nRF5 SDK · Python |
| [**weather_lora_link**](https://github.com/zainnmiann/weather_lora_link) | Solar weather station to gateway over LoRa P2P, with HMAC-signed frames, a relay hop and a cellular uplink. Range-tested in the field | C++ · ESP32 · Wio-E5 · MQTT |
| [**jetson-human-detection**](https://github.com/zainnmiann/jetson-human-detection) | Real-time YOLO11 person detection on a Jetson AGX Orin running Yocto, with MP4 recording and a live web view | Python · PyTorch · OpenCV · systemd |
| [**uwb_bridge**](https://github.com/zainnmiann/uwb_bridge) | Raspberry Pi service that streams UWB ranges from UART to MQTT, with framing, checksums and auto-recovery | Python · MQTT · systemd |
| [**esp32_uwb_tdma_twr**](https://github.com/zainnmiann/esp32_uwb_tdma_twr) | ESP32 UWB Pro port of the multi-tag, multi-anchor ranging protocol | C/C++ · PlatformIO |
| [**WeatherStation**](https://github.com/zainnmiann/WeatherStation) | ESP32 station: BME280, AS3935 lightning detector, wind/rain kit, soil moisture | Arduino · ESP32 |
| [**gta4-macos**](https://github.com/zainnmiann/gta4-macos) | How I got GTA IV running on an Apple Silicon Mac | Wine · macOS |

### Toolbox

**Languages**&nbsp;
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

**Embedded**&nbsp;
![nRF52](https://img.shields.io/badge/nRF52-00A9CE?style=flat-square&logo=nordicsemiconductor&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=flat-square&logo=platformio&logoColor=white)
![UWB](https://img.shields.io/badge/UWB-DW1000-555555?style=flat-square)
![LoRa](https://img.shields.io/badge/LoRa-P2P-555555?style=flat-square)

**Edge & infra**&nbsp;
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![NVIDIA Jetson](https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Yocto](https://img.shields.io/badge/Yocto-555555?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

**ML & vision**&nbsp;
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-555555?style=flat-square)
![Kalman](https://img.shields.io/badge/Kalman_filtering-555555?style=flat-square)
