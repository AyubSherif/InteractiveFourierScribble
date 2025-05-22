# 🎨 Interactive Fourier Scribble

This educational tool is an **interactive Fourier series visualizer**, designed to help users intuitively understand how Fourier approximations work in representing arbitrary signals.

I built this tool for my mom's physics class (My mom is a **physics professor**).

---

## 🔧 How It Works

1. The user draws a signal using their mouse.
2. The signal is sampled and interpolated to a uniform grid.
3. A discrete Fourier transform is computed using `numpy.fft`.
4. Only the selected number of modes (harmonics) are kept.
5. The inverse transform reconstructs the signal from those modes.
6. The original and approximated signals are plotted together.

### Launch on Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AyubSherif/InteractiveFourierScribble/main?urlpath=%2Fdoc%2Ftree%2FInteractiveFourierScribble.ipynb)

---

## 🔍 What It Illustrates

1. Fourier Decomposition of Functions:

    - It shows how any drawn signal (even non-standard ones) can be approximated by summing a finite number of sine and cosine terms—i.e., Fourier modes.

    - The "Fourier Modes" slider lets users control how many harmonics are used in the reconstruction, revealing how approximation quality improves with more terms.

2. Signal Reconstruction and Convergence:

    - It illustrates how low-order approximations capture only the basic shape or average of the signal.

    -  As the number of modes increases, finer details and sharper features emerge—demonstrating convergence of Fourier series.

---

## 🖼️ Sample Output

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
