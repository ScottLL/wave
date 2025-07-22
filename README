# Wave: Audio Visualisation & Cymatics Playground

![Cymatics demo](123.gif)

## Overview
Wave is a lightweight collection of Python notebooks for experimenting with digital audio signals and visualising their hidden patterns in both 2-D and 3-D.  Think of it as an interactive playground where you can:

- Inspect waveforms from existing `.wav` files.
- Capture live microphone audio and perform real-time spectral analysis.
- Generate mesmerising Chladni ("cymatic") patterns that reveal the geometry of standing sound waves.

Whether you are a musician, a physics enthusiast, or simply curious about sound, this repository gives you an approachable starting point for hands-on exploration.

---

## Features

| Notebook | What it demonstrates |
|----------|----------------------|
| `wave_test.ipynb` | Reads a stereo `.wav`, separates channels, and plots the raw waveform. |
| `wave_3d.ipynb`  | Captures microphone input, computes an FFT, and translates dominant frequencies into dynamic Chladni patterns. |

Additional assets:

- **`audio/sample-15s.wav`** – Short royalty-free clip for quick testing.
- **`123.gif`** – Example animation generated from the cymatics notebook.

---

## Project Structure
```
wave/
├── audio/                # Sample audio assets
│   └── sample-15s.wav    # 15-second test file
├── wave_test.ipynb       # Waveform exploration
├── wave_3d.ipynb         # Cymatics generator
├── 123.gif               # Demo animation
└── LICENSE               # MIT License text
```

---

## Requirements

- **Python 3.10+** (tested with 3.11)
- Recommended: a virtual environment (`venv`, `virtualenv`, or `conda`).
- The notebooks themselves install missing packages on-the-fly, but you can pre-install them manually:

```bash
pip install numpy matplotlib scipy pygame pyaudio jupyterlab
```

> **Note for macOS users:** `pyaudio` depends on PortAudio. Install using Homebrew before `pip`:
> ```bash
> brew install portaudio
> ```

---

## Quick Start

1. Clone the repository and enter the project folder:
   ```bash
   git clone https://github.com/<your-username>/wave.git
   cd wave
   ```
2. Create & activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt  # or use the one-liner above
   ```
4. Launch Jupyter and open a notebook:
   ```bash
   jupyter lab  # or: jupyter notebook
   ```
5. Run the cells.  Feel free to tweak parameters like `m`, `n`, and `frequency_factor` in `wave_3d.ipynb` to craft new patterns.

---

## Using Your Own Audio

1. Drop a `.wav` file (44.1 kHz or 48 kHz recommended) into the `audio/` directory.
2. In `wave_test.ipynb`, change the `wave.open()` path to your file.
3. Re-run the notebook to analyse and plot your signal.

Live input from your microphone is handled automatically inside `wave_3d.ipynb`—no additional steps needed.

---

## Troubleshooting

| Issue | Possible fix |
|-------|--------------|
| *PyAudio fails to install* | macOS: `brew install portaudio` • Windows: install [official wheels](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio) |
| *No audio device detected* | Ensure microphone permissions are granted to the terminal/Jupyter app |
| *Plots appear blank* | Verify your backend supports interactive plotting (`matplotlib inline` or `%matplotlib widget`) |

---

## Contributing

Pull requests are welcome!  If you have new visualisation ideas, optimisations, or bug fixes:

1. Fork the repo.
2. Create a feature branch: `git checkout -b feature/my-awesome-idea`.
3. Commit your changes with clear messages.
4. Open a PR describing **what** and **why**.

Please keep new functions under 50 lines and document them thoroughly.

---

## License

This project is released under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Inspired by the historic Chladni figures and modern cymatics research.
- Uses open-source libraries: NumPy, SciPy, Matplotlib, PyAudio, and Pygame.

Enjoy making waves! 🌊🎵
