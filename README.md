
# Mor Braz – Data Processing

This project provides a Jupyter Notebook to process data from the Mor Braz acquisition campaign. The boat is equipped with a thermosalinograph and a GPS tracker.

## Overview

The notebook allows you to merge and interpolate data from the onboard instruments, then export the results to the `output` folder.

## Requirements

- Python 3.7 or higher
- [virtualenv](https://python-guide-pt-br.readthedocs.io/fr/latest/dev/virtualenvs.html#virtualenv)
- Jupyter Notebook

## Installation

1. **Clone the repository:**

   ```bash
   git clone git@github.com:astrolabe-expeditions/MorBraz.git
   cd MorBraz
   ```

2. **Create a Python virtual environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

   For Windows with Powershell
   ```
   .\venv\Scripts\Activate.ps1
   ```

   If `virtualenv` is not installed, follow the [documentation](https://python-guide-pt-br.readthedocs.io/fr/latest/dev/virtualenvs.html#virtualenv).

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   pip install notebook
   ```

4. **Start Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

5. **Open the notebook file:**
   - In your browser, open `interpolate_data_with_track.ipynb`.

## Usage

1. Launch Virtual Environnement
   ```
   .\venv\Scripts\Activate.ps1
   ```
2. Start Jupyter Notebook
   ```
   jupyter notebook
   ```
1. Place your data files in the `input` folder.
2. Update the variables in the notebook to match your file names.
3. Run the notebook cell by cell.
4. Check the exported result in the `output` folder.
5. Save the generated file wherever you need.

## Folder Structure

- `input/`: raw data files (CSV, GPX, etc.)
- `output/`: exported results after processing
- `interpolate_data_with_track.ipynb`: main notebook
- `requirements.txt`: Python dependencies
