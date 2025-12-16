# E-Ink Weather Display

Low-power ESP32 weather station with e-ink display. Updates every 30 minutes, shows current conditions with minimal battery drain.

## Hardware

- ESP32 development board
- Waveshare 2.13" 3-color e-ink display (212x104, red/black/white)
- Connections: CS=15, DC=27, RST=26, BUSY=25, MOSI=14, CLK=13

## Features

- Current temperature & feels-like
- Weather icon
- Precipitation probability
- High/Low forecast
- Wind speed (when ≥20 km/h)
- Animated dinosaur (burn-in prevention)
- Deep sleep between updates (30 min)
- Smart refresh (only updates when weather changes)

## Setup

1. Install Arduino IDE with ESP32 support
2. Install libraries: `GxEPD2`, `ArduinoJson`
3. Get free API key from [OpenWeatherMap](https://openweathermap.org/api)
4. Edit code:
   - `ssid` = your WiFi name
   - `password` = your WiFi password
   - `apiKey` = your OpenWeatherMap key
   - `city` = your city name
5. Upload to ESP32

## Battery Life

With 2500mAh battery: ~2-3 months (depending on WiFi connection time)

## License

MIT
