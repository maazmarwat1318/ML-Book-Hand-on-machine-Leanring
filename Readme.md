# Running Jupyter Notebooks with Virtual Environment (venv)

## 📌 Prerequisites

Make sure you have the following installed:

- **Python 3.x** (Recommended: Latest version)
- **pip** (Python package manager)
- **VS Code** (if using VS Code for Jupyter notebooks)

## 🚀 Setting Up the Virtual Environment

Follow these steps to create and activate a virtual environment:

### 1️⃣ Create a Virtual Environment

```sh
python -m venv .venv
```

This will create a `.venv` folder in your project directory.

### 2️⃣ Activate the Virtual Environment

- **Windows (PowerShell):**
  ```sh
  .venv\Scripts\Activate
  ```
- **Mac/Linux:**
  ```sh
  source .venv/bin/activate
  ```

### 3️⃣ Install Dependencies

Make sure Jupyter is installed inside the virtual environment:

```sh
pip install jupyter
```

Install all requirements in requirements.txt file:

```sh
pip install -r requirements.txt
```

## 📝 Running Jupyter Notebook

Once the virtual environment is activated, start Jupyter Notebook:

```sh
jupyter notebook
```

This will open Jupyter Notebook in your web browser.

## 🎯 Running Jupyter in VS Code

If you're using **VS Code**, follow these steps:

1. Open **VS Code** in your project folder.
2. Open the **Command Palette** (`Ctrl + Shift + P`).
3. Search for and select **"Python: Select Interpreter"**.
4. Choose the one with .venv in it's name will most likely look like **Python 3.x.x('.venv')**.
5. Open a `.ipynb` file and select the **.venv** kernel at the top right.
6. Start running your notebook! 🚀

## 🔄 Deactivating the Virtual Environment

When you're done, you can deactivate the virtual environment with but remeber if installing packages you must install them when virtual environment is activated:

```sh
deactivate
```

## ✅ Verifying Jupyter Kernel

To ensure Jupyter is using the correct Python environment, run this inside a notebook:

```python
import sys
print(sys.executable)
```

It should output a path ending in `.venv/Scripts/python.exe`.

---

Now you're ready to work with Jupyter notebooks in an isolated virtual environment! 🎉
