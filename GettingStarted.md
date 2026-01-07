# Getting Started (Computer Lab)

For the labs and final project, you can run Python code in **one of two ways**:

## Option 1: Google Colab (recommended for getting started)
Google Colab is a free online notebook environment that runs in your browser.

- Colab is a great option for Lab 1 because it works immediately (no installation needed).
- Colab has limited computing resources, but that should **not** be an issue for our class labs and projects.

## Option 2: Run locally on your computer
Running locally means installing Python, Jupyter Notebook, and the required packages on your machine.

- This gives you more control and fewer limitations.
- It takes a bit longer to set up the first time, but it is worth it if you plan to keep using these tools.

---

# Lab 1 Requirements

For Lab 1, you will use the following Python packages:

```python
import numpy as np
import pandas as pd
import altair as alt

from sklearn.neighbors import KNeighborsRegressor
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error
````

---

# Using Google Colab (Online)

1. Go to Google Colab and create a new notebook.
2. Upload the lab notebook (`.ipynb`) or open it from Google Drive.
3. If any package is missing, install it in a notebook cell:

```python
!pip install numpy pandas altair scikit-learn
```

---


# Running Locally using Anaconda

Some students prefer **Anaconda** because it installs Python, Jupyter, and many data science packages in one step.

* This can be easier if you have never installed Python packages before.
* The downside is that it is a larger install, its take more storage and can be a little slugish.

If you already use Anaconda, that is perfectly fine for this class.

(If you choose Anaconda, you can launch Jupyter Notebook from Anaconda Navigator, or by running `jupyter notebook` in the Anaconda Prompt/terminal.)

---

# Running Locally (Alternative Setup: No Anaconda)

## 1) Install Python

Download Python from:
[https://www.python.org/downloads/](https://www.python.org/downloads/)

**Windows users:** during installation, make sure you check:

* ✅ **“Add Python to PATH”**

To confirm Python is installed, open a terminal and run:

```bash
python --version
```

If that does not work, try:

```bash
python3 --version
```

---

## 2) Install Jupyter Notebook (without Anaconda)

Open **Terminal** (Mac/Linux) or **Command Prompt / PowerShell** (Windows), then run:

```bash
python -m pip install notebook
```

If your computer uses `python3`, run:

```bash
python3 -m pip install notebook
```

### Launch Jupyter Notebook

In the terminal, go to the folder where your lab files are located (optional), then run:

```bash
jupyter notebook
```

This should open a new tab in your web browser showing the Jupyter file browser.

To stop Jupyter:

* Press **CTRL + C** in the terminal (then type `y` if prompted).

---

## 3) Install the Lab 1 Packages

Run the following command in your terminal:

```bash
python -m pip install numpy pandas altair scikit-learn
```

If your computer uses `python3`, run:

```bash
python3 -m pip install numpy pandas altair scikit-learn
```

---

## 4) Quick Setup Check (Recommended)

After installing, open a notebook and run:

```python
import numpy as np
import pandas as pd
import altair as alt
from sklearn.neighbors import KNeighborsRegressor

print("Setup works!")
```

If you see `Setup works!`, you are ready for Lab 1.

---


# Common Fix (Permission Errors)

If you get permission errors when installing packages, try:

```bash
python -m pip install --user notebook
```

or

```bash
python -m pip install --user numpy pandas altair scikit-learn
```

