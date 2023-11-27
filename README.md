# talon-voice-quizzes

## Purpose
Interactive quizzes to refresh recall of Talon Voice commands.
Recall of these commands fades in several days after first exposure to them.
The recall decreases more slowly with repeated exposure.
This quiz supports improving the recall.

A PDF version of each quiz is provided for those who are unable to run the interactive version of the quiz.


## Disclaimer
This is a programming tool, not an educational tool.
It provides no explanations and no context.
The `quiz` impoves recall of computer commands in a quote manner.


## Prerequisites
You need a recent version of Python3.
You also need one external module.
Install the module **pytictoc** with pip or conda.

```bash
pip install --user --upgrade pytictoc
```

or with conda

```bash
conda activate <env name>
conda install pytictoc
```

If you have an older version of python3, install the module **tictoc** instead.

## Run one of two ways.

You will be asked to enter a number between 1 and 1. Enter 1.
Then the interactive quiz will run.

### Run in terminal

```bash
./qTalon<subtopic>.py
```

Enter control-D to interupt the quiz.

### Run in Jupyter
Use in Jupyter Notebook, JupyterLab, [JupyterLab.app](https://blog.jupyter.org/jupyterlab-desktop-app-now-available-b8b661b17e9a), or nteract.app.
Probably works in Colab, too, but you may have to load the quiz onto your Google Drive.
Select the approprite Python kernel that taps into the Python interpreter with pytictoc installed.

The advantages of this approach is that the results can be stored in the Notebook and it is more fun to run the quiz in Jupyter.

Check on present working directory in Jupyter by entering the following in a code cell.

```bash
!pwd
```

The file qVoiceTyping.py must be in your working direcotry or you must give the full file path to qVoiceTyping.py.
Enter the following in another code cell.

```bash
%run -i "qVoiceTyping.py"
```
