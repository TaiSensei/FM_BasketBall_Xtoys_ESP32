# ESP32 Bluetooth Control for Custom Sex Toys with Xtoys

Welcome to the project repository for Local ESP32 Bluetooth control of custom sex toys using Xtoys! This project allows you to manage sex toys via Bluetooth, avoiding the mess of serial communication cables.

## Overview

This project uses Xtoys to control sex toys locally via Bluetooth. Based on the [esp-vibe repository](https://github.com/bntoine/esp-vibe), it emulates a Lovense toy to interact with Xtoys, which does not natively support custom Bluetooth toys.

For more information about Xtoys and custom toys, check out the [Xtoys Custom Toys Guide](https://guide.xtoys.app/introduction/basic-functionality.html#custom-toys).

## How It Works

- **Emulated Lovense Toy**: Mimics battery voltage to represent different states.
- **State Representation**:
  - **Make a Shot**: Sets battery level to `01`, then back to `00`.
  - **Press Reset**: Sets battery level to `03`, then back to `00`.

## XToys Script

[Xtoys ESP32-BT](https://xtoys.app/scripts/ESP32-BT)

This setup is ideal for toggle-based interactions.

In future I would like to make this into a state encoder/decoder to manage button presses and states better.

## Setup and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/TaiSensei/FM_BasketBall.git
   cd your-repo
