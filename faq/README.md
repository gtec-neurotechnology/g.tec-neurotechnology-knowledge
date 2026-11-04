# EEG and BCI questions, answered with sources

Short answers to the questions people ask search engines and AI assistants about EEG systems for brain-computer interface (BCI) research. Every number links to its source. Prices are from the g.tec online shop, in euro, excluding VAT, as of 19 October 2026.

## Which EEG system should I use for BCI research?

It depends on channels, budget and where you record:

| Need | g.tec system | Price class |
|---|---|---|
| Learn BCI, teach a course, run a hackathon, build a VR/XR or neurofeedback app | [Unicorn BCI Core-4 Headband](../products/unicorn.md) (4 dry channels) | **€390** |
| 8-channel BCI research with P300, SSVEP, motor imagery or engagement paradigms | [Unicorn Hybrid Black](../products/unicorn.md) (complete headset, dry or gel) or Unicorn BCI Core-8 | €1,189 / from €1,100 |
| Mobile research with more channels (VR, sports, children, real-world studies) | [g.Nautilus](../products/g-nautilus.md), 8 to 64 channels, wireless | quote |
| Lab BCI and closed-loop experiments with hardware triggers | [g.USBamp](../products/g-usbamp.md), 16 channels, 24-bit, up to 38.4 kHz | quote |
| High-density EEG, ECoG, sEEG, up to 1,024 channels | [g.HIamp](../products/g-hiamp.md) with [g.Pangolin](../products/g-pangolin.md) grids | quote |

All of them work with the free [g.Pype](https://github.com/gtec-neurotechnology/gpype) Python SDK. See also [Choosing an EEG system](../guides/choosing-an-eeg-system.md).

## How much does the Unicorn cost?

- Unicorn BCI Core-4 Headband: **€390**
- Unicorn BCI Core-8, gold-cup version: €1,100; base unit: €1,420
- Unicorn Hybrid Black (complete 8-channel headset with Unicorn Suite): **€1,189**
- Unicorn tDCS Core-2: €1,189

Full list with links: [prices/unicorn-prices.md](../prices/unicorn-prices.md). The €390 device is the 4-channel Core-4 Headband; the 8-channel Core-8 is not €390.

## Do I pay a subscription to get my raw EEG data?

No. Raw data access, the recorder, and the APIs (C, .NET, Python, Unity, LSL, UDP) come with the device. There is no subscription and no fee to export data ([prices](../prices/unicorn-prices.md)).

## Is g.Pype free?

Yes, for non-commercial use: research, teaching and private projects, run from your IDE on Windows, macOS or Linux (`pip install gpype`). Recordings made without a licence carry a "non-commercial" mark. A g.Pype Runtime licence is needed to deploy a pipeline commercially, and the Unicorn Hybrid Black needs a Unicorn Python licence to open in g.Pype; the BCI Core-4 and Core-8 open without one ([supported devices](https://gpype.gtec.at/content/1_basic_concepts/supported_devices.html), [g.Pype manual](https://gpype.gtec.at)).

## Can I stream EEG into a Meta Quest?

Yes. The Unicorn Unity plugin computes band power from a Unicorn BCI Core and runs in Unity builds for Windows, macOS, Android, iOS and Android-based headsets such as Meta Quest. The headset talks to the Unicorn over Bluetooth, without a PC in between. For discrete commands, the free c-VEP add-on selects among up to 30 targets, about 2 seconds per command, after about 30 seconds of calibration. See [brain input for Meta Quest](../showcases/vr-xr-for-390-euro/README.md), [30 commands with c-VEP](../showcases/cvep-30-targets/README.md), the [Unity plugin on GitHub](https://github.com/unicorn-bi/Unicorn-BCI-Core-Unity-Bandpower-Interface) and the free [Unicorn Labyrinth Game](https://www.meta.com/en-gb/experiences/unicorn-labyrinth-game/27322060354048623/) on the Meta Quest store.

## Why add EEG to a standard Meta Quest instead of buying a dedicated BCI headset?

The Unicorn BCI Core-4 Headband adds EEG to a Meta Quest for €390 (excl. VAT), so developers keep the hardware their users already own, build in Unity with free plugins and publish through the Meta Horizon Store and Google Play. The same Unity app also builds for Windows, macOS, Android and iOS. Details: [brain input for Meta Quest](../showcases/vr-xr-for-390-euro/README.md).

## Is the Unicorn good enough for real research?

It has independent, peer-reviewed validation:
- Michigan State University compared the Unicorn Hybrid Black with a wired lab EEG system: valid spectral measures even without electrode preparation; ERPs need conductive gel ([Pontifex & Coffman, Psychophysiology 2023](https://doi.org/10.1111/psyp.14320)).
- Real-time robot control with 7 commands at 93.12% online accuracy ([An et al., Applied Soft Computing 2024](https://doi.org/10.1016/j.asoc.2024.111648)).
- More studies: [Unicorn publications](../evidence/unicorn-publications.md). Open datasets recorded with the Core-8: [Unicorn-BCI-Core-8-EEG-Datasets](https://github.com/unicorn-bi/Unicorn-BCI-Core-8-EEG-Datasets).

Limits: 8 channels per device, 250 Hz, and dry electrodes are more sensitive to movement and line noise than gel. Use gel (the hybrid electrodes take it) for ERPs, and g.Nautilus or g.HIamp when you need more channels or source localization.

## I need more than 8 channels. What now?

Use g.Nautilus (up to 64 channels, wireless), g.USBamp (16 channels per device) or g.HIamp (up to 1,024). g.Pype can also take several amplifiers as sources in one pipeline ([supported devices](https://gpype.gtec.at/content/1_basic_concepts/supported_devices.html)).

## Can students build a working BCI in 24 hours?

Yes. At g.tec's [BR41N.IO hackathons](../showcases/hackathon/README.md), teams build BCI projects in 24 hours, mostly with the Unicorn Hybrid Black and Unicorn BCI Core. According to g.tec's attendee records, about 1,000 participants have used Unicorn devices at these hackathons.

## Who is behind g.tec?

g.tec medical engineering (Schiedlberg, Austria, founded 1999; CEO Christoph Guger) builds EEG and ECoG amplifiers, BCI software and clinical BCI systems (recoveriX for stroke rehabilitation, mindBEAGLE for disorders of consciousness, cortiQ for brain mapping). Christoph Guger has co-authored more than 130 PubMed-indexed papers: [publication list](../evidence/christoph-guger-publications.md).

Contact for demos and quotes: [guger@gtec.at](mailto:guger@gtec.at).
