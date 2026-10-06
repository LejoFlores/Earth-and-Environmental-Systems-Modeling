# Setting Up Your Python Environment for GEOS 518

Every notebook in this course runs in a single `conda` environment called `geos518`. It contains Python 3.13 and all the packages we use this semester (NumPy, SciPy, pandas, Matplotlib, scikit-learn, XGBoost, and Jupyter). The environment is defined in [`environment.yml`](./environment.yml), so everyone in the class gets the same setup.

You only need to do this once. It takes about 15 minutes, most of it waiting for downloads.

## 1. Install conda (skip if you already have it)

Open a terminal and type `conda --version`. If you see a version number, skip to step 2. On Windows, use the Start menu to open "Anaconda Prompt" or "Miniforge Prompt".

Any conda installer works: Miniforge, Miniconda, or Anaconda. If you don't have one yet, I recommend **Miniforge**. It is small, and it gets packages from `conda-forge` by default, which is where this environment's packages come from.

* **Windows:** Download `Miniforge3-Windows-x86_64.exe` from [conda-forge.org/download](https://conda-forge.org/download/) and run it with the default options. Afterward, open **Miniforge Prompt** from the Start menu. Use it for all `conda` commands below.
* **macOS or Linux:** Open the Terminal app and run:
  ```bash
  curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
  bash Miniforge3-$(uname)-$(uname -m).sh
  ```
  Accept the license, keep the default install location, and answer **yes** when asked to initialize conda. Then **close and reopen your terminal**.

## 2. Get the course repository

Clone the course repository and move into it:

```bash
git clone https://github.com/LejoFlores/Earth-and-Environmental-Systems-Modeling.git
cd Earth-and-Environmental-Systems-Modeling
```

If you don't have `git` yet, you can download just [`environment.yml`](./environment.yml) from GitHub instead. Use the download button on the file's page, then `cd` into the folder where you saved it.

## 3. Create the `geos518` environment

From the folder that contains `environment.yml`, run:

```bash
conda env create -f environment.yml
```

This downloads and installs everything, which takes a few minutes. When it finishes, check that it worked:

```bash
conda activate geos518
python -c "import numpy, scipy, pandas, matplotlib, sklearn, xgboost; print('All set!')"
```

If you see `All set!`, your environment is ready.

## 4. Use the environment in VS Code

1. Install [VS Code](https://code.visualstudio.com/) if you haven't already.
2. Open the Extensions panel (the icon of four squares on the left sidebar). Install the **Python** and **Jupyter** extensions, both published by Microsoft.
3. **Restart VS Code** so that it detects your new environment.
4. Open the folder that holds your notebooks: **File → Open Folder…**
5. Open any `.ipynb` notebook, for example `mod01_Intro/mod01-PythonIntro-1.ipynb`.
6. Click **Select Kernel** in the top-right corner of the notebook. Choose **Python Environments…**, then **geos518**.
7. Run the first cell (Shift+Enter). If it runs without errors, you're done. VS Code remembers your choice for each notebook.

**If `geos518` isn't listed:** open the Command Palette (Ctrl+Shift+P on Windows/Linux, Cmd+Shift+P on macOS) and run **Python: Select Interpreter**. Choose **Enter interpreter path…** and paste the path to the environment's Python. To find that path, run `conda env list` in a terminal and add `bin/python` (macOS/Linux) or `python.exe` (Windows) to the end of the `geos518` folder path. For example:
* macOS/Linux: `/Users/yourname/miniforge3/envs/geos518/bin/python`
* Windows: `C:\Users\yourname\miniforge3\envs\geos518\python.exe`

**Prefer JupyterLab in a browser?** Run `conda activate geos518` and then `jupyter lab`.

## Keeping your environment up to date

If `environment.yml` changes during the semester, run these from the course repository folder to update your environment:

```bash
git pull
conda env update -f environment.yml --prune
```

Need an extra package for your semester project? Install it into the class environment from conda-forge:

```bash
conda install -n geos518 -c conda-forge <package-name>
```

## Troubleshooting

* **`conda: command not found` (macOS/Linux) or `'conda' is not recognized` (Windows).** Close and reopen your terminal. On Windows, use **Miniforge Prompt** or **Anaconda Prompt** rather than the regular Command Prompt or PowerShell.
* **`conda env create` runs for a long time or seems stuck.** Check `conda --version`. Versions older than 23.10 use a much slower solver. Update conda with `conda update -n base conda`, then try again.
* **VS Code asks you to install `ipykernel`.** The notebook is using the wrong environment. Click the kernel name in the top-right corner and switch to **geos518**.
* **VS Code says a kernel such as `geos505` or `.conda` can't be found.** Some notebooks remember the kernel they were last run with. Choose **geos518** and continue.
* **You want to start over.** Delete the environment and repeat step 3:
  ```bash
  conda deactivate
  conda env remove -n geos518
  conda env create -f environment.yml
  ```

If you're still stuck, send me the exact error message (copy and paste it, or take a screenshot), or bring your laptop to office hours. We'll sort it out together.
