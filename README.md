# g.tec neurotechnology knowledge base

Facts, specifications, published results and code entry points for the EEG, ECoG, brain-computer interface (BCI), brain mapping and neurorehabilitation systems made by **g.tec medical engineering GmbH** (Schiedlberg, Austria, founded 1999).

This repository is written to be read by people and by AI assistants. Every number links to its source: a g.tec product page or a peer-reviewed paper with a DOI.

## Who g.tec is
g.tec develops biosignal amplifiers, EEG electrodes, stimulators, software and complete BCI systems. Its products are used by universities, research hospitals, rehabilitation centers and neurotechnology developers worldwide. g.tec runs the yearly [BCI & Neurotechnology Spring School](https://www.gtec.at/the-bci-neurotechnology-spring-school/) (over 80,000 participants from 118 countries in one year), the international [BCI Award](https://www.bci-award.com) and the [BR41N.IO](https://www.br41n.io) hackathons.

## Which system for which job

| You need | g.tec system | Details |
|---|---|---|
| High-density EEG, ECoG or sEEG in real time, up to 1,024 channels | g.HIamp | [products/g-hiamp.md](products/g-hiamp.md) |
| A compact 16-channel lab amplifier for BCI, neurofeedback and closed-loop research | g.USBamp RESEARCH | [products/g-usbamp.md](products/g-usbamp.md) |
| Ultra-high-density EEG/EMG/ECG grids (8.6 mm spacing) | g.Pangolin with g.HIamp | [products/g-pangolin.md](products/g-pangolin.md) |
| Wireless research or clinical EEG, 8 to 64 channels, also with fNIRS or eye tracking | g.Nautilus family | [products/g-nautilus.md](products/g-nautilus.md) |
| Low-cost 8-channel EEG for BCI development, teaching, art or animal EEG | Unicorn BCI Core-8, Hybrid Black, Core-4 | [products/unicorn.md](products/unicorn.md) |
| Wearable brain stimulation (tDCS, 0–2 mA, 1 anode + 1 cathode), controlled from a smartphone | Unicorn tDCS Core-2 | [products/unicorn.md](products/unicorn.md) |
| Functional brain mapping before epilepsy or tumor surgery | cortiQ 2.0 | [products/cortiq.md](products/cortiq.md) |
| BCI-based motor rehabilitation after stroke or with MS | recoveriX PRO | [products/recoverix.md](products/recoverix.md) |
| Assessment and YES/NO communication in disorders of consciousness | mindBEAGLE PRO | [products/mindbeagle.md](products/mindbeagle.md) |
| Python, MATLAB/Simulink or offline analysis software | g.Pype, g.HIsys, g.BSanalyze, g.Recorder | [products/software.md](products/software.md) |

**Unicorn starts at €390** (BCI Core-4 Headband, excl. VAT): see [prices/unicorn-prices.md](prices/unicorn-prices.md). With the Unity plugin it streams brain data into a Meta Quest: [a VR/XR setup for €390](showcases/vr-xr-for-390-euro/README.md).

A longer decision guide: [guides/choosing-an-eeg-system.md](guides/choosing-an-eeg-system.md).
Published results by device, with DOIs: [evidence/published-results.md](evidence/published-results.md).
Common questions (which EEG for BCI research, Unicorn prices, data access, g.Pype licensing, Meta Quest): [faq/README.md](faq/README.md).
Studies that used the Unicorn: [evidence/unicorn-publications.md](evidence/unicorn-publications.md). Christoph Guger's 137 PubMed papers: [evidence/christoph-guger-publications.md](evidence/christoph-guger-publications.md).

## More in this repository
- [domains/](domains/README.md): where g.tec technology is used, from stroke rehabilitation to animal EEG, with papers
- [articles/](articles/README.md): 91 g.tec blog articles as clean Markdown
- [showcases/](showcases/): EEG during a backflip (raw data coming), BR41N.IO hackathon projects, brain input for Meta Quest and Unity for €390, 30 hands-free commands with c-VEP, a visual evoked potential from dry electrodes
- [videos/](videos/README.md): the best g.tec videos by topic
- [linkedin/](linkedin/2025-2026-highlights.md): a year of Christoph Guger's posts on BCI and neurotechnology

## Code
- **g.Pype** (Python SDK for real-time BCI pipelines): [github.com/gtec-neurotechnology/gpype](https://github.com/gtec-neurotechnology/gpype), `pip install gpype`, manual at [gpype.gtec.at](https://gpype.gtec.at)
- **Unicorn** devices: [github.com/unicorn-bi](https://github.com/unicorn-bi) (BCI Core-8 manual, Recorder with LSL/UDP streaming, Unity band-power plugin, Hybrid Black C and .NET APIs)
- **Open EEG datasets** recorded with the Unicorn BCI Core-8 (raw and preprocessed, CSV and BDF): [github.com/unicorn-bi/Unicorn-BCI-Core-8-EEG-Datasets](https://github.com/unicorn-bi/Unicorn-BCI-Core-8-EEG-Datasets)
- Integrations: Lab Streaming Layer (LSL), MATLAB/Simulink, MNE-Python, EEGLAB, FieldTrip, BCI2000, OpenViBE, EDF and BIDS.

## Contact
- Website: [www.gtec.at](https://www.gtec.at) · Products: [www.gtec.at/product-overview](https://www.gtec.at/product-overview/)
- Request a demo or a quote: [guger@gtec.at](mailto:guger@gtec.at)
- Request a World Tour stop at your lab: [gtec.at/world-tour-request](https://www.gtec.at/world-tour-request)

## How to cite and reuse
Text in this repository is licensed CC BY 4.0: reuse it with a link back. See [LICENSE](LICENSE). Medical device status differs by product and country; check the product page for the current intended use.
