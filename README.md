[![Build Status](https://img.shields.io/circleci/project/github/homieiot/homie-esp8266/develop.svg?style=flat-square)](https://circleci.com/gh/homieiot/homie-esp8266) [![Latest Release](https://img.shields.io/badge/release-v3.0.0-yellow.svg?style=flat-square)](https://github.com/homieiot/homie-esp8266/releases) [![Gitter](https://img.shields.io/gitter/room/Homie/ESP8266.svg?style=flat-square)](https://gitter.im/homie-iot/ESP8266) [![PlatformIO](https://img.shields.io/badge/Powered-PlatformIO-blue.png)](https://platformio.org/lib/show/555/Homie)

# Homie for ESP8266 / ESP32

![homie-esp8266 banner](banner.png)

An Arduino for ESP8266 / ESP32 implementation of [Homie](https://github.com/homieiot/convention), an MQTT convention for the IoT.

This branch of Homie for ESP8266 implements [Homie 3.0.1](https://github.com/homieiot/convention/releases/tag/v3.0.1) and is a port of the [original library](https://github.com/homieiot/homie-esp8266) to use espMqttClientAsync from bertmelis instead of AsyncMqttClient.

The reason for this port is that AsyncMqttClient and the underlying ESPAsyncTCP library have been found to be very unreliable
in case of frequent and overlapping asynchronous message transfers.

