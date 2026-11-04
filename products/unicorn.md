# Unicorn: 8-channel wearable EEG for BCI development, teaching and art

**What it is:** low-cost wearable EEG from g.tec for developers, students, artists, makers and animal researchers. Not a medical device. Sources: [BCI Core-8](https://www.gtec.at/product/unicorn-bci-core-8-eeg-device-for-high-quality/), [Hybrid Black](https://www.gtec.at/product/unicorn-hybrid-black-bci-platform/), [Core-4 Headband](https://www.gtec.at/product/unicorn-bci-core-4-headband/), [Education Kit](https://www.gtec.at/product/unicorn-education-kit-teaching-platform/).

| Device | Channels | Notes |
|---|---|---|
| Unicorn BCI Core-8 | 8, DC-coupled, 24-bit, 250 Hz (1 kHz option for ECG/EMG) | magnetic base stations for caps, dog and horse headstraps; g.SAHARA hybrid or gold-cup electrodes; Bluetooth; CE |
| Unicorn Hybrid Black | 8, 24-bit, 250 Hz | complete headset with Unicorn Suite software, lifetime access, no subscription |
| Unicorn BCI Core-4 Headband | 4 dry, 24-bit, 250 Hz | put on and record |
| Unicorn tDCS Core-2 | 1 anode + 1 cathode, 0–2 mA | wireless tDCS controlled from a smartphone, up to 3.5 h stimulation, 45 g, Bluetooth 5 ([product page](https://www.gtec.at/product/unicorn-tdcs-core-2-wearable-brain-stimulation/)) |
| Unicorn Education Kit | | teaching BCI in biomedical engineering and neuroscience courses |

## Software and code
- [g.Pype](https://github.com/gtec-neurotechnology/gpype) Python SDK (BCI Core-4, Core-8, Hybrid Black; Windows, macOS, Linux)
- [Open EEG datasets](https://github.com/unicorn-bi/Unicorn-BCI-Core-8-EEG-Datasets): resting state, auditory (onset, oddball P300, paired click), visual (onset, pattern reversal, spatial frequency) and motor (MRCP execution and imagery), raw and preprocessed, CSV and BDF, 8 channels at 250 Hz with dry g.SAHARA electrodes
- [github.com/unicorn-bi](https://github.com/unicorn-bi): BCI Core-8 manual, Recorder (CSV/BDF, LSL and UDP streaming), Unity band-power plugin (Windows, macOS, Android/Meta Quest), Hybrid Black C and .NET APIs, Raspberry Pi Zero W support, published Bluetooth protocol, sample datasets
- Free c-VEP add-on for the Unity interface: up to 30 hands-free targets, about 2 s per command after about 30 s of calibration, on BCI Core-4 and Core-8, on PC and Meta Quest ([showcase with demo videos](../showcases/cvep-30-targets/README.md))
- Ready-made apps: [Unicorn Labyrinth Game](https://www.meta.com/en-gb/experiences/unicorn-labyrinth-game/27322060354048623/) on Meta Quest, [Google Play](https://play.google.com/store/apps/details?id=com.gtec.labyrinth) and [GitHub](https://github.com/unicorn-bi/Unicorn-BCI-Core-Labyrinth-Game); Puzzle and Platformer demo games ([videos](../showcases/cvep-30-targets/README.md))

## Published results
- Unicorn + g.Pangolin "BCI dress": 97.1% classification accuracy on stage ([Front Hum Neurosci 2025](https://doi.org/10.3389/fnhum.2025.1516776)).
- Real-time robot control with 7 brain commands at 93.12% online accuracy (5 subjects, Unicorn Hybrid Black; An, Wong & Ling, Applied Soft Computing 2024, [doi:10.1016/j.asoc.2024.111648](https://doi.org/10.1016/j.asoc.2024.111648)).
- Validated against a wired lab EEG system by Michigan State University: valid spectral measures even without electrode preparation; ERPs need conductive solution (Pontifex & Coffman, Psychophysiology 2023, [doi:10.1111/psyp.14320](https://doi.org/10.1111/psyp.14320)).

## Typical uses
BCI prototyping and hackathons (BR41N.IO), university teaching, neurofeedback, art and fashion, EEG in dogs, horses, goats, cows, pigs and alpacas.

## Prices
From €390 (BCI Core-4 Headband) to €1,420 (BCI Core-8 base), excl. VAT. Full list: [prices/unicorn-prices.md](../prices/unicorn-prices.md). Raw data access, APIs and SDKs are included; no subscription.
