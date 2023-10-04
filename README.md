# TOTE PATTERN GENERATOR

## Installation

### For macOS Ventura

Download repository:

```bash
cd /path/to/directory # e.g., /Users/handmadephd/Documents/github
git clone https://github.com/HandmadePhD/tote-pattern.git
cd tote-pattern
```

Set path to your virtual environment. For example:

```bash
MY_PYENV=/Users/handmadephd/Applications/pyenv/
mkdir ${MY_PYENV}/tote-pattern
```

Install virtual python environment:

```bash
virtualenv ${MY_PYENV}/tote-pattern --python=python3.11
```

Activate new virtual environment:

```bash
source ${MY_PYENV}/tote-pattern/bin/activate
```

Install required python packages provided in this repository:

```bash
python -m pip install -r requirements.txt
```

Run Jupyter Notebooks:

```
jupyter notebook
```

### For Windows 11 using Powershell

Install **pyenv-win** using Powershell since pyenv is only for UNIX-based systems:

```powershell
Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
```

Download repository:

```powershell
cd \path\to\directory # e.g., C:\Users\handmadephd\Documents\github
git clone https://github.com/HandmadePhD/tote-pattern.git
cd tote-pattern
```

Set path to your virtual environment. For example:

```powershell
mkdir $home\virtualenvironments\pyenv\tote-pattern
```

Install virtual python environment:

```powershell
virtualenv $home\virtualenvironments\pyenv\tote-pattern --python=python3.11
```

Activate new virtual environment:

```powershell
$home\virtualenvironments\pyenv\tote-pattern\Scripts\activate.ps1
```

Install required python packages provided in this repository:

```powershell
python -m pip install -r requirements.txt
```

Run Jupyter Notebooks:

```powershell
jupyter notebook
```

## Usage
Open the *.ipynb file.

Change the following variables according to your preferred bag dimension.

```
# height of bag in inches from bottom to top
HGT = 12

# width of bag from side to side
WID = 10

# depth of bag from front to back
DEP = 9

# sewing seam allowance
SMA = 0.25

# top double fold hem
HEM = 0.625
```

Happy coding!