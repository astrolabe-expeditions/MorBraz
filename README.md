
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

If `virtualenv` is not installed, follow the [documentation](https://python-guide-pt-br.readthedocs.io/fr/latest/dev/virtualenvs.html#virtualenv).

   ```bash
   python -m venv venv
   ```

1. **Launch Virtual Environnement:**

   For Windows with Powershell

   ```bash
   .\venv\Scripts\Activate.ps1
   ```

   Or for Unix based system (Linux, macOS)

   ```bash
   source venv/bin/activate
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   pip install notebook
   ```

## Usage

1. **Launch Virtual Environnement:**

   For Windows with Powershell

   ```bash
   .\venv\Scripts\Activate.ps1
   ```

   Or for Unix based system (Linux, macOS)

   ```bash
   source venv/bin/activate
   ```

2. **Start Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

3. **Open the notebook file:**
   - In your browser, open `interpolate_data_with_track.ipynb`.
4. Place your data files in the `input` folder.
5. Update the variables in the notebook to match your file names.
6. Run the notebook cell by cell.
7. Check the exported result in the `output` folder.
8. Save the generated file wherever you need.

## Folder Structure

- `input/`: raw data files (CSV, GPX, etc.)
- `output/`: exported results after processing
- `interpolate_data_with_track.ipynb`: main notebook
- `requirements.txt`: Python dependencies
