![Version](https://img.shields.io/static/v1?label=talon-voice-quizzes&message=0.1&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

# talon-voice-quizzes

## Purpose
Interactive quizzes to refresh recall of Talon Voice commands.
Recall of these commands fades in several days after the first exposure to them.
The recall decreases more slowly with repeated exposure.
This quiz supports improving the recall.

A PDF version of each quiz is provided for those who cannot run the interactive version.

## Features

- Randomizes questions on each run
- Reports the number of correct answers
- Reports time spent on quiz

## Disclaimer
This is a programming tool, not an educational tool.
It provides no explanations and no context.
The `quiz` improves recall of computer commands in a quote manner.


## Prerequisites
You need a recent version of Python3.
You also need one external module.
Install the module **pytictoc** with pip.

```bash
pip install --user --upgrade pytictoc
```

or with a conda environment

```bash
conda activate <env name>
pip install --upgrade pip 
pip install pytictoc
```

If you have an older version of python3, install the module **tictoc** instead.

## Run one of two ways.

You will be asked to enter a number between 1 and 1. Enter 1.
Then the interactive quiz will run.

### Run in terminal

```bash
./qTalon<subtopic>.py
```

Enter control-D to interrupt the quiz.

### Run in Jupyter
Use in Jupyter Notebook, JupyterLab, [JupyterLab.app](https://blog.jupyter.org/jupyterlab-desktop-app-now-available-b8b661b17e9a), or [nteract.app](https://nteract.io/).
The last two options are stand-alone desktop applications that do not use the browser.
You still need a Python3 kernel mapped to a Python interpreter with the module `pytictoc` installed via pip.
Probably works in Colab, too, but you may have to load the quiz onto your Google Drive.
Select the appropriate Python kernel that taps into the Python interpreter with pyritic installed.

The advantages of this approach are that the results can be stored in the Notebook and that running the quiz in Jupyter is more fun.

Check on the present working directory in Jupyter by entering the following in a code cell.

```bash
!pwd
```

The file qVoiceTyping.py must be in your working directory, or you must give the full file path to qVoiceTyping.py.
Enter the following in another code cell.

```bash
%run -i "qVoiceTyping.py"
```
