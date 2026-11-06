# Fnirsi-DOPX180H-DPX
Unofficial FNIRSI DPOX180H firmware extension and Windows software: USB screen capture, waveform analysis, FFT, measurements, remote control and automated tests.

**Project author: Sergey Patsinko**

An unofficial project for the **FNIRSI DPOX180H** oscilloscope, combining modified firmware **4.05.0** with the **DPX Snapshot** application for Windows.

The project enables data exchange between the oscilloscope and a PC, remote control, recording, and signal analysis.

## Features

- Oscilloscope screen capture over USB.
- Waveform acquisition in min/max format.
- Reading the instrument’s measurements from both channels, including RMS.
- Remote operation of the instrument’s buttons.
- Built-in signal generator control through the instrument’s existing button handlers.
- Saving waveforms, CSV files, and measurement sessions.
- Zooming, panning, and cursor measurements.
- Additional PC-side calculations, waveform math, and FFT.
- Event detection and recording with pre-event history.
- Automated tests using configurable scenarios.
- Russian, English, and Chinese user interfaces.

## Software and Firmware

The PC application and instrument firmware use independent version numbers:

- **DPX Snapshot** — the Windows application.
- **4.05.0** — the modified oscilloscope firmware.
- **V40** — the original factory firmware provided for rollback.

Installers and ready-to-use packages are available in the **Releases** section.

## Acquisition Limitations

The transferred waveform array contains processed min/max data, rather than a continuous stream of raw ADC samples.

Gaps may occur between individual captures. A recorded session must not be treated as a gapless signal recording. Timing calculations and FFT results should be assessed with regard to the settings and resolution of the selected capture.

## Documentation

The documentation covers software and driver installation, firmware updates, rollback to the factory firmware, operation of the instrument, and a description of the modifications.

A technical firmware change register is available in Russian, English, and Chinese.

## Feedback

Please report bugs and submit suggestions in the **Issues** section.

When reporting a bug, include:

- PC application and firmware versions.
- Windows version.
- Steps to reproduce the issue.
- Expected and actual behavior.
- A screenshot or recording file, if it helps reproduce the problem.

## Credits

Firmware modifications and PC software: **Sergey Patsinko**.

Original factory firmware and hardware platform: **FNIRSI**.

This is an independent project and is not an official FNIRSI product.
