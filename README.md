![Circuit Diagram](extras/ogjjs81y.png)                ![Device Photo](extras/wd5ta6pj33.png)

# Zigbee Converter for iHseno Human Presence Sensor

[![GitHub license](https://img.shields.io/github/license/yourusername/ihseno-presence-sensor-converter)](LICENSE)
[![Zigbee2MQTT](https://img.shields.io/badge/Zigbee2MQTT-supported-blue)](https://www.zigbee2mqtt.io/)

Converter for integrating the iHseno Human Presence Sensor (model `_TZE284_debczeci`) with Zigbee2MQTT.

## Supported Devices
- iHseno Human Presence Sensor ([AliExpress Link](https://www.aliexpress.com/item/1005009110929003.html))

## Features
- Human presence detection
- Battery level monitoring
- Adjustable PIR sensitivity (low/medium/high)
- Configurable PIR delay time (15s/30s/60s)

## Installation
1. Copy the `tuya_tze284_pir.js` file to your Zigbee2MQTT `external_converters/` directory
2. Restart Zigbee2MQTT

## Supported Features
| Feature | Description |
|---------|-------------|
| `presence` | Presence detection (true/false) |
| `battery` | Battery level in percentage |
| `pir_sensitivity` | PIR sensitivity (low/medium/high) |
| `pir_time` | PIR delay time (15s/30s/60s) |

## Example Zigbee2MQTT Configuration
```yaml
devices:
  '0x1234567890abcdef':
    friendly_name: presence_sensor_living_room
    retain: false
