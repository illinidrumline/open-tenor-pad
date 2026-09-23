<!-- SPDX-FileCopyrightText: 2026 Illini Drumline contributors -->
<!-- SPDX-License-Identifier: MIT -->

# Firmware

Sensor firmware for the electronic tier (v2). Empty for now.

Planned direction:

- One piezo per zone plus a rim sensor, on an ESP32-S3 or Teensy 4.x.
- A trigger engine in the class of [edrumulus](https://github.com/corrados/edrumulus):
  positional sensing, retrigger cancellation, rimshot and choke detection, crosstalk
  cancellation, clipping compensation, target under 10 ms latency.
- USB-MIDI and BLE-MIDI output.

Not started. v0 is acoustic-only.
