# auto-refresh-latex
How to set up real-time Latex editing on OS X using existing tools.

## Installation
1. [MacTex](http://www.tug.org/mactex/)
2. [Skim PDF Editor](http://skim-app.sourceforge.net/)
3. [Sublime Text](https://www.sublimetext.com/)
4. [Python](https://www.python.org/)

## Skim
Enable "Check for file changes" under preferences. This will auto-update your PDF view whenever the underlying PDF changes.

## When-Changed
Run the following:

  ```$ pip install https://github.com/joh/when-changed/archive/master.zip```

## Auto-Save
Install package manager on Sublime. Then install the [auto-save package](https://packagecontrol.io/packages/auto-save). Turn it on by creating a new keybinding (I choose ctrl-shift-s).

## Start Editing!
1. Run the following:

   ```$ when-changed CV.tex pdflatex CV.tex```
2. Open up Sublime and Skim side by side. Start editing code in Sublime - the PDF view in Skim should automatically update as you type.
