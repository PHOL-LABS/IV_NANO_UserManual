# IV-Indicators Nano User Manuals

[![CI](https://github.com/Sgw32/DR_UserManuals/actions/workflows/main.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/main.yml)
[![CI (French)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/french.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/french.yml)
[![CI (German)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/german.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/german.yml)
[![CI (Hungarian)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/hungarian.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/hungarian.yml)
[![CI (Russian)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/russian.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/russian.yml)
[![CI (Spanish)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/spanish.yml/badge.svg)](https://github.com/Sgw32/DR_UserManuals/actions/workflows/spanish.yml)

This repository hosts the LaTeX sources for the official documentation shipped with every IV-Indicators Nano gauge set.  The manuals describe the modular indicator family that covers Golf 2, Jetta 2, Golf 1, Jetta 1, Polo, and Audi 80 B2 installations.  They are kept in sync with the production firmware, configuration utilities, and wiring harnesses supplied with the devices.

## 📘 What is inside

- **Fundamental safety guidance** describing how to handle the programmer, power the indicators, and avoid damage to the electronics.
- **Device overview** summarizing the IV-Indicators variants (voltmeter, barometer, thermometer, lambda, boost) and the compatible sensors shipped or recommended for each option.
- **Configuration walkthroughs** for the IV-Conf Android beta app and the IV-Conf web pack, including preset management and calibration adjustments.
- **Reference appendices** that consolidate sensor characteristics, temperature tables, and reflashing instructions.

The compiled PDF (`IV_Indicators_User_Manual.pdf`) is the master document used for customer deliveries.  Each section of the manual lives in the `chapters/` directory, supporting data and macros reside in `preamble/`, while ancillary assets (figures, tables, and scripts) are stored under `figures/` and `anc/`.

Localized builds are published alongside the English edition: French (`_fr`), Russian (`_ru`), Hungarian (`_hu`), German (`_de`), and Spanish (`_es`).  Each translation currently carries placeholder text so that outdated Digifiz content is removed while the new wording is being prepared.

## 🚗 Vehicle coverage

IV-Indicators Nano modules are designed for the following Volkswagen Group classics:

- **Volkswagen Golf Mk2 (1983–1992)**
- **Volkswagen Jetta Mk2 (1984–1992)**
- **Volkswagen Golf Mk1**
- **Volkswagen Jetta Mk1**
- **Volkswagen Polo (86C)**
- **Audi 80 B2 (1978–1986)**

Adapters for additional models will be documented as compatibility is confirmed.

## 🛠️ Building the manual locally

1. Install a recent TeX distribution (TeX Live 2025 or newer is recommended) that includes `latexmk`, `pdflatex`/`lualatex`, and `biber`.
2. For the automated figure pipeline, also install `inkscape`, `perl`, `sed`, `uconv`, and `ghostscript`.  These utilities enable vector export and watermark generation used in the PDF.
3. Clone this repository and run:

   ```sh
   latexmk IV_Indicators_User_Manual
   ```

   The command builds `IV_Indicators_User_Manual.pdf` in the repository root.  Clean builds (`latexmk -C`) and alternative engines can be configured in `.latexmkrc`.

If you prefer cloud editing, you can upload the project to Overleaf.  Select the latest TeX Live compiler and ensure shell-escape is enabled for chapters that render SVG figures.

## 🤝 Community and support

For hardware sales, installation services, or manual feedback, reach out to PHOL-LABS Kft via the contact information supplied with your order.  Community channels for IV-Indicators Nano will be announced alongside firmware milestones.

## 💖 Support the project

- **PayPal:** `sgw32nc@gmail.com`
- **Crypto (ETH / USDT ERC-20):** `0xeDc17cb23241eACe19DF3617291aa7d2d92E62DC`
- **3D printed accessories and models:** [cgtrader.com/sgw32](https://www.cgtrader.com/sgw32)

## 🧾 License

Documentation sources in this repository are released under the [Creative Commons CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) dedication (see `LICENSE`).

## ™️ Trademarks

Volkswagen, Audi, and their respective vehicle names are trademarks of Volkswagen AG and Audi AG.  References are provided solely for identification of compatible vehicles.  IV-Indicators Nano is produced by PHOL-LABS Kft and is not affiliated with the OEMs listed above.
