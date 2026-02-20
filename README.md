# Boardsource Wireless Corne SMT Firmware

This repository contains the official ZMK configuration for the **Wireless Corne SMT**. This PCB is designed for a seamless, cable-free experience with full support for ZMK Studio.

* **Product Page:** [Wireless Corne SMT PCB](https://boardsource.xyz/products/wireless-corne-smt-pcb-assembled-hot-swap-zmk-compatible-split-keyboard-pcb)
* **Full Documentation & Build Guide:** [Wireless SMT Corne Docs](https://boardsource.xyz/blogs/guides/wireless-smt-corne-docs)

---

## Features

* **ZMK Studio Ready:** Change your keymap in real-time without reflashing.
* **Fully Wireless:** No TRRS cable or USB connection required for standard use.
* **Universal Support:** Works with MX, Choc v1, and Choc v2 switches.
* **Pre-Flashed:** Ready to use out of the box.

---

## Expansion Pinout

The 8-pin header on each side (identical, not mirrored) is read from left to right. These are perfect for screens (nice!view / e-ink) or custom hardware.

| Pin | GPIO | Note |
| --- | --- | --- |
| 1 | 0.07 |  |
| 2 | 0.21 |  |
| 3 | 0.12 |  |
| 4 | 0.23 |  |
| 5 | VCC | Switched via pin 0.31 |
| 6 | GND |  |
| 7 | 0.19 |  |
| 8 | 0.05 |  |

---

## Battery Information

If shipping allows, batteries are included. The PCB features a micro JST connector (BM02B-ACHSS-GAN-ETF) and labeled solder pads (+/-) for custom installs.

**Max Dimensions:**

* **Choc:** 30x17x3mm
* **MX:** 30x17x6mm

---

## Flashing

1. Edit `config/blecorne.keymap`
2. Push -> GitHub Actions builds automatically
3. Download `.uf2` from Actions -> Artifacts
4. USB -> double tap reset -> drag `.uf2` to the drive
5. Flash both halves separately (`_left` and `_right`)

## Links

- [Miryoku](https://github.com/manna-harbour/miryoku)
- [Wireless SMT Corne Docs](https://boardsource.xyz/blogs/guides/wireless-smt-corne-docs)
- [ZMK Docs](https://zmk.dev/docs)
