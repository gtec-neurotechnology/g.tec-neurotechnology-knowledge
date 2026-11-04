# g.tec software

| Software | What it does | Language |
|---|---|---|
| [g.Pype](https://gpype.gtec.at) | SDK for real-time and offline BCI and neuroscience pipelines; node-based; supports Unicorn, g.Nautilus, g.USBamp, g.HIamp (+ g.Pangolin), LSL and UDP; Windows, macOS, Linux; `pip install gpype` | Python 3.10–3.14 |
| [g.HIsys Professional](https://www.gtec.at/product/ghisys-biosignal-acquisition-analysis/) | real-time development environment for BCI, closed-loop and stimulation experiments | MATLAB/Simulink |
| [g.BSanalyze](https://www.gtec.at/product/gbsanalyze-offline-eeg-analysis/) | offline analysis: OSCAR PRO artifact correction, ERP, ERD/ERS, time-frequency, classification, batch processing | MATLAB-based |
| [g.Recorder](https://www.gtec.at/product/biosignal-recording-software/) | recording and signal quality for EEG, TMS-EEG, wireless EEG, evoked potentials | GUI |
| [g.tec Suite 2024](https://www.gtec.at/product/gtec-suite-2024-software/) | acquisition, processing, recording, analysis and BCI application development in one package | |
| [Unicorn Suite](https://www.gtec.at/product/unicorn-suite/) | user-ready and programmable apps for Unicorn Hybrid Black | C, .NET, Unity, LSL |

**OSCAR LIVE** removes movement, muscle and eye artifacts in real time.

## Quick start with g.Pype (no hardware needed)
```shell
pip install "gpype[all]"
git clone https://github.com/gtec-neurotechnology/gpype.git
```
Then run `examples/s1e2_hello_world.py`. The built-in signal generator lets a pipeline run without an amplifier. Full manual for LLMs: [gpype.gtec.at/llms-full.txt](https://gpype.gtec.at/llms-full.txt).
