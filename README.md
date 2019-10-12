# M5StickC YUN-HAT with ambient

## Overview

ENV visualizing program for M5Stick YUN-HAT. and logging data to ambient cloud.

[original code is here](https://github.com/m5stack/M5-ProductExampleCodes)

## Requirements

- [M5StickC](https://m5stack.com/collections/m5-core/products/stick-c)
- [M5StickC Yun Hat(SH20,BMP280,SK6812)](https://m5stack.com/products/m5stickc-yun-hatsh20-bmp280-sk6812)

## Preapre to use

- 2.4Ghz WiFi AP with Internet connectivity
- Setup your env
    - Arduino IDE
        - ESP32 board lib
        - M5StickC lib
        - Adafruit_BMP280 lib
    - CP210x USB to Serial Driver
        - https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Windows.zip
- Setup your ambient channel
    - https://ambidata.io
    - sign up
    - create channel
    - get `Channel ID` and `Write Key`

## Config

1. Create `hat-yun/env.h` file. [hat-yun/.env.h](./hat-yun/.env.h) is template for `env.h` file.
1. modify `env.h` file.
    - WiFi SSID and Password
    - ambient Channel ID and Write Key

## Run code

1. Verify and Upload [hat-yun.ino](./hat-yun/hat-yun.ino) to M5StickC
1. Insert M5StickC to YUN-HAT
