# Machine Learning for Robotics

Course materials, assignments, and environment setup notes for the Machine Learning for Robotics track. Use this repo to follow along with class sessions, practice exercises, and set up a consistent Python environment on Windows or Ubuntu.

## Repository Layout
- `0. Environment Setup/01. Windows/` — Windows installation notes, Git/GitHub setup, and Python virtual environment steps.
- `0. Environment Setup/02. Ubuntu/` — Ubuntu installation notes, Git/GitHub setup, and Python virtual environment steps.
- `01. Class 1/01. RECML_ Class 01.pdf` — Class 1 slides.
- `01. Class 1/02. Assignment/ML_Class01_Practice_Questions.pdf` — Class 1 practice questions.
- `02. Class 2/01. RECML_ Class 02.pdf` — Class 2 slides.
- `02. Class 2/02. NumPy Cheat Sheet.pdf` — Quick reference for NumPy basics.
- `02. Class 2/03. Exercise.pdf` — Class 2 exercises.
- `02. Class 2/04. Solutions.pdf` — Suggested solutions for Class 2 exercises.

## Quick Start (Python Environment)
1) Install Python 3.10+ and VS Code.
2) From the project root, create a virtual environment:
   - Ubuntu: `python3 -m venv .venv && source .venv/bin/activate`
   - Windows (PowerShell): `python -m venv .venv; .\\.venv\\Scripts\\Activate.ps1`
3) Install core packages:
   ```bash
   pip install --upgrade pip
   pip install numpy pandas matplotlib scikit-learn jupyter ipykernel
   ```
4) (Optional, for deep learning/GPU) Install PyTorch:
   ```bash
   pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
   ```
5) Register the Jupyter kernel (while the venv is active):
   ```bash
   python -m ipykernel install --user --name=ml --display-name="ML (.venv)"
   ```
6) In VS Code, run `Python: Select Interpreter` and choose the `.venv` interpreter.

## Git and GitHub Tips
- Everyday workflow and branch basics are documented in:
  - `0. Environment Setup/01. Windows/02.1. Git and Github Tutorial.md`
  - `0. Environment Setup/02. Ubuntu/02.1. Git and Github Tutorial.md`
- VS Code GitHub sign-in and publish steps are covered in:
  - `0. Environment Setup/01. Windows/02. Git and Github Integration.md`
  - `0. Environment Setup/02. Ubuntu/02. Git and Github Integration.md`

## Working With the Materials
- Slides and PDFs can be opened directly from the paths above.
- Keep notebooks or scripts you create alongside the class folders or in a new `notebooks/` folder inside the repo.
- When starting a new session, activate `.venv` first so your imports and kernels use the pinned environment.
