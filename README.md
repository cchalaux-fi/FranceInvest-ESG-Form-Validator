# France Invest ESG Form Validator

The **France Invest ESG Form Validator** is a local web application (runs on your computer) that **checks Excel (.xlsx) files** against the machine‑readable rules of the **France Invest ESG framework**.

It helps you detect:
- missing required fields,
- invalid formats or values,
- structural issues in the workbook.

> The app runs locally: your files are not uploaded to the internet.

---

## Quick start (3 steps)

1. Open a terminal and go to the project folder  
2. Install dependencies  
3. Start the app and open the local URL in your browser

Details below.

---

## 1) Requirements

You need:
- **Windows / macOS / Linux**
- **Python 3** installed (recommended: **Python 3.13**)
- An Excel file to validate (**.xlsx**)

---

## 2) Download the project

Download (or clone) the project source code into a single folder, for example:
- Windows: `Documents\FI_ESG_Validator\`
- macOS: `Documents/FI_ESG_Validator/`

⚠️ Keep **all project files together** in the same folder (do not move individual files out of the folder).

---

## 3) Install Python (if needed)

### Check whether Python is installed

Open a terminal and run:

- Windows:
  ```bash
  python --version
  ```
- macOS / Linux:
  ```bash
  python3 --version
  ```

If you see something like `Python 3.x.x`, you’re good.

### Install Python

Download Python here:
https://www.python.org/downloads/

**Windows important note:** during installation, check **“Add Python to PATH”**.  
Otherwise the `python` command may not work.

---

## 4) Open a terminal

### Windows
Open **PowerShell**:
- Start menu → type `PowerShell` → Enter

### macOS
Open **Terminal**:
- Applications → Utilities → Terminal

### Linux
Open your **Terminal** application.

---

## 5) Go to the project folder

In the terminal, move into the folder where the project is located.

Examples:

### Windows (PowerShell)
```powershell
cd "C:\Users\YOUR_NAME\Documents\FI_ESG_Validator"
```

### macOS / Linux
```bash
cd /Users/YOUR_NAME/Documents/FI_ESG_Validator
```

Tip: you can often **drag and drop the folder** into the terminal to insert its path.

---

## 6) Install dependencies (one-time setup)

The validator needs a few Python libraries.

### Step 1 — install the dependencies
```bash
pip3 install -r requirements.txt
```

### If `pip3` does not work

Try one of these alternatives:

- Windows:
  ```bash
  pip install -r requirements.txt
  ```
- Or:
  ```bash
  python -m pip install -r requirements.txt
  ```
- macOS / Linux:
  ```bash
  python3 -m pip install -r requirements.txt
  ```

---

## 7) Start the application

From the project folder, run:

### macOS / Linux
```bash
python3 "France Invest ESG Validator.py"
```

### Windows
```powershell
python "France Invest ESG Validator.py"
```

> The filename must match exactly what you see in the project folder.  
> If the main script has a different name on your side, replace it accordingly.

When the app is running, the terminal usually shows something like:
- `Running on http://127.0.0.1:5000/`

---

## 8) Open the app in your browser

Open your browser (Chrome, Edge, Firefox…) and go to:

**http://127.0.0.1:5000/**

You should see the validator interface. Upload/select a `.xlsx` file to validate it.

---

## 9) Stop the application

To stop the server:
- go back to the terminal
- press **Ctrl + C**

---

## Troubleshooting

### “python is not recognized” (Windows)
Python is not installed or not added to PATH.  
Reinstall Python and check **“Add Python to PATH”**.

### “No module named flask” (or another missing module)
Dependencies were not installed (or you installed them in another environment).  
Run step 6 again from the project folder.

### “Address already in use” (port 5000)
Another program is already using port 5000 (or the validator is already running).  
Stop the other instance (Ctrl + C) or close the other terminal.

---

## Notes
- Only **.xlsx** files are supported.
- The tool runs locally on your machine.
