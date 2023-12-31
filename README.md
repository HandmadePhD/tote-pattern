# Tote Bag Pattern Generator

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
Open the *.ipynb file from the jupyter notebook window.

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

# Depending on your bag dimensions, the text on the image may render poorly.
# You can increase or decrease the value of f to adjust the size of your image.
# Larger f-values gives more room for the text.
# Smaller f-values gives less room for the text.
# Set f anywhere between 1 and 1000.
f = 30
```

Once you've edited your measurements, click `Run > Run All Cells`.

The pattern is saved in your current working directory, which should be `/Users/handmadephd/Documents/github/tote-pattern`. You can view a sample pattern here: [HandmadePhD_tote_12H_10W_9D_0.625HEM_0.25SA.png](HandmadePhD_tote_12H_10W_9D_0.625HEM_0.25SA.png). The file is saved with the dimension information.

Happy coding!