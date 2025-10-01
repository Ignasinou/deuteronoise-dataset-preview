# DeuteroNoise Database — Open Website Dataset (Preview)

> **Status:** Early preview of the forthcoming **DeuteroNoise** open website dataset.  
> This repository hosts a small, curated sample of audio recordings, metadata, and
> visualizations (spectrograms & SPL plots) to allow reviewers to evaluate the
> project before the full website and complete dataset go live.

---

## 🔍 Overview

The **DeuteroNoise Database** is a **multi-basin, calibrated underwater sound dataset**
with paired AIS vessel information. It was designed to support research on
anthropogenic noise in the marine environment.

Key features:

- **Calibrated acoustic recordings** (48 kHz / 24-bit) from multiple campaigns:  
  *Barcelona (Badalona & Espai Vela), Venice Lagoon, Black Sea (Mamaia & Constanța)*.
- **Noisy vs quiet** site pairs enabling impact comparisons.
- **AIS-linked vessel metadata** (MMSI, vessel type, speed, range).
- **Open licensing** for reproducible research (MIT for code, CC-BY 4.0 for data/plots).

This repo is a **preview** — the full dataset and web platform (searchable,
filterable, with an interactive viewer) will be released on the upcoming
DeuteroNoise website.

---

- **`data/campaigns`** — sample campaigns with WAV snippets, metadata, and example plots.  
- **`taxonomy_vessel_types.csv`** — simple vessel type lookup table.  
- **`docs/demo_video.mp4`** — short video demo of the upcoming web interface.

---

## 🗂️ Campaign samples

| Campaign | Basin / Country | Site type |
|----------|-----------------|-----------|
| 2023-12_BCN_Badalona_Q | Catalan Coast, Spain | Quiet |
| 2024-03_BCN_EspaiVela_N | Catalan Coast, Spain | Noisy |
| 2024-03_IT_Venice_QN   | Venice Lagoon, Italy | Mixed |
| 2024-09_RO_Mamaia_Q    | Black Sea, Romania   | Quiet |
| 2024-09_RO_Constanta_N | Black Sea, Romania   | Noisy |

Each campaign folder contains:

- Short **audio files** (`audio_*.wav` — placeholder or real samples)
- `metadata.csv` with:  
  `start_time, end_time, mmsi, vessel_type, sog_knots, range_m, basin, country, site_label`
- **Spectrograms** (`spectrograms/*.png`) — time/frequency visualizations
- **SPL plots** (`spl_plots/*.png`) — overall or 1/3-octave band sound pressure levels

---

## 🎥 Demo video

A short screen-capture of the planned **Streamlit-based website** is provided:

<p align="center">
  <img src="docs/demo_video.mp4" alt="Demo video placeholder" width="600"/>
</p>

---

## ⚖️ License

- **Data & plots**: [CC BY 4.0](LICENSES/LICENSE-CC-BY-4.0.txt)  
- **Code snippets / repository structure**: [MIT](LICENSES/LICENSE-MIT.txt)

---

## 🌐 Full website (coming soon)

The complete database with all audio, metadata, and interactive search tools
will be hosted at:

**<https://deuteronoise.eu>** *(placeholder URL — replace with your real site)*
