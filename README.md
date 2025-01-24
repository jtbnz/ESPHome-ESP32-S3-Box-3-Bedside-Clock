# ESPHome ESP32-S3 Box 3 Bedside Clock

A smart bedside clock built with ESPHome and the ESP32-S3 Box 3 development kit. Features a touch-enabled display with multiple pages and smart home controls.

    README GENERATED by Copilot

## Hardware Components
- ESP32-S3 Box 3 with built-in display and touch screen
- DHT temperature/humidity sensor
- BH1750 light sensor

## Features

### Display Interface
- Three swipeable pages:
  1. Main Page: Clock display with smart home controls
  2. Weather Page: Temperature and humidity readings
  3. Status Page: Device information and light sensor readings

### Smart Home Controls
- Four touch buttons for controlling:
  - Bedroom lights
  - Bed head light
  - Heat pump
  - Electric blankets
- Button states sync with Home Assistant
- Touch buttons use Material Design icons

### Ambient Light Adaptation
- BH1750 sensor monitors room brightness
- Automatically adjusts screen brightness:
  - Dims to 30% below 50 lux
  - Full brightness above 50 lux

### Power Management
- Screen can be turned off using the home button
- Screen timeout feature (configurable from 10-180 seconds)

### Time and Updates
- Syncs time with Home Assistant
- Updates display every minute
- Supports OTA (Over-The-Air) updates

### Environmental Monitoring
- Temperature and humidity readings every 60 seconds
- Light level readings every 30 seconds

### Network
- WiFi connection with fallback AP mode
- Captive portal for easy setup
- Home Assistant API integration with encryption

## Touch Controls
- Swipe left/right in the clock area to change pages
- Home button toggles display on/off
- Touch anywhere to wake the display
