# 🎨 Interactive Fourier Scribble

This Jupyter Notebook is an **educational tool** I built as a class project to visualize how **Fourier series** can be used to approximate arbitrary signals.

---

## 🚀 How It Works

1. The user draws a signal using their mouse.
2. The signal is sampled and interpolated to a uniform grid.
3. A discrete Fourier transform is computed using `numpy.fft`.
4. Only the selected number of modes (harmonics) are kept.
5. The inverse transform reconstructs the signal from those modes.
6. The original and approximated signals are plotted together.

---

**First Fourier Mode (Function Average)**

![First Mode](https://github.com/AyubSherif/InteractiveFourierScribble/blob/main/img/FirstMode.png)

**Fourth Fourier Mode**

![Fourth Mode](https://github.com/AyubSherif/InteractiveFourierScribble/blob/main/img/FourthMode.png)

**20th Fourier Mode**

![20th Mode](https://github.com/AyubSherif/InteractiveFourierScribble/blob/main/img/20thMode.png)

**100th Fourier Mode**

![100th Mode](https://github.com/AyubSherif/InteractiveFourierScribble/blob/main/img/100thMode.png)

---

## 📦 Required Python Packages

To run the notebook, install the following:

```bash
pip install ipympl numpy matplotlib ipywidgets
or
pip install -r requirements.txt
