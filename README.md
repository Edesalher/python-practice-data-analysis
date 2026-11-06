# Python Data Analysis Practice

This repository documents a 10-day study plan for practicing data analysis with Python in Jupyter notebooks. The goal is to explore datasets, calculate metrics, and interpret results to answer business questions.

I use Claude as a tutor to suggest exercises, ask me questions about my analysis, and evaluate my conclusions.

## Repository Structure

- `dia_XX.ipynb` — daily exercise notebooks in the repository root. The notebooks are a work in progress and will be added or updated as I work through the plan.
- `notas/` — analysis notes for days when I write them.
- [`CLAUDE_README.md`](CLAUDE_README.md) — the prompt I used to ask Claude to be my tutor and create the study plan.
- `data/` — the local folder for the source datasets, excluded from version control.

## Datasets

| Dataset | Description | Filename in `data/` |
| --- | --- | --- |
| [Chinook Database](https://github.com/lerocha/chinook-database) | A sample database for a digital music store. This practice uses the SQLite version. | `Chinook_Sqlite.sqlite` |
| [Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail) | Transaction data from a UK-based online retailer. | `Online Retail.xlsx` |

## Running the Notebooks

1. Clone this repository and open a terminal in its root directory.
2. Create a `data/` directory. Download the SQLite version of Chinook and the Online Retail spreadsheet from the sources above. Extract the files if needed and save them in `data/` using the filenames shown in the table.
3. Create and activate a Python virtual environment. Using a dedicated `.venv` is recommended so that the notebooks and their dependencies use the same Python environment.

   **Linux or macOS**

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

   **Windows (PowerShell)**

   ```powershell
   py -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

4. Install the required packages from the activated environment.

   ```bash
   pip install --upgrade pip
   pip install pandas numpy matplotlib seaborn jupyterlab openpyxl
   ```

5. Open a notebook using either option.

   - **JupyterLab.** With `.venv` active, run `jupyter lab` from the repository root and open a `.ipynb` file in your browser.
   - **VS Code.** Install the [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) and [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) extensions. Open the repository folder and a `.ipynb` file, then use **Select Kernel** to choose the `.venv` environment.

6. Run the notebook cells in order.

## Acknowledgments

- **`Chinook_Sqlite.sqlite`** — Luis Rocha and the Chinook project contributors. [Documentation and source files](https://github.com/lerocha/chinook-database) · [Release downloads](https://github.com/lerocha/chinook-database/releases)
- **`Online Retail.xlsx`** — Daqing Chen. [Dataset details and source file at the UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail)
