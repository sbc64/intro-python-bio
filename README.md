# Intro to python bio

This document assumes you have no experience with python or the commandline and will hopefully point you in the right direction. To get started with the nitty gritty go to: [Your first program!](#your-first-program) or read ["Introduction To Programming Using Python"](#books)

This guides jumps straight into programming python and I hope it has enough to get someone started. You can safely skip the Github and Pipenv sections. I do recommend that to learn Python you find something you want to work on.

## Why python?

Why python and not R? I think they are both great! They have incredibly strong support in bioinformatics. The only advantage I see with python is that you can use it for other programming areas that R might not be as good at such as machine learning. Learning either R or Python is not mutually exclusive. They are both similar in how to program. From my limited brief exposure to R, the main differences is that R has built in dataframes while with python you need to install the Pandas library to handle data frame.

Also, from my view point you can learn either Python or R and be a proficient developer but Python will give better understanding in the long run about what is programming. This make spicking up R easier in the future.

## Github

__NOTE Github is not neccesary for you to learn python. But it will be helpful tool when you are working with more than two people. You can skip this part__

The first step is to make a github account: https://github.com/join?source=header-home

And then follow some bioinformatians:
- https://github.com/BenLangmead
- https://github.com/johanneskoester
- https://github.com/dcjones
- https://github.com/sjackman

Following people allows you to  discover what they like and you might something interesting.

You should also download https://desktop.github.com/

Why git?: 
- https://programminghistorian.org/en/lessons/retired/getting-started-with-github-desktop

## Programming environment/Setup

### IDE (Integrated development environment)

Install VSCode: https://code.visualstudio.com/

Why VScode? It is the most simple IDE but at the same time it is the most powerful when extensions get added. Other IDEs have way too many buttons and you can easily get lost. In the end you can learn how to use python with just a commandline and a text file. But we don't want to be that extreme.

### Python3

Just use Python 3 everywhere. Avoid Python 2
Install: https://docs.python-guide.org/starting/install3/osx/

### Pipenv

__NOTE Pipenv is not a neccesary tool, but like github it will avoid some pains in the future. You can ignore it for now since it is not neccesary but I find it important to know that it exists__

Pipenv is a tool to make each project you work on have different python libraries without interfeering on the other libraries. Sometimes you can have two libraries. Say `csv-parser` and `csv-parser-3000` and they both use a different common library called `dictionary-handler-2000` but different versions. If you install both csv libraries at the system level they will both be stepping over each installing the different versions of `dictionary-handler-2000`. It is not strictly neccesary but I highly recommend it.

https://pipenv.readthedocs.io/en/latest/#install-pipenv-today

Usage will look like this. Open the VSCode terminal of the new project:

```
pipenv shell
```

That is it. Then you can `pip install <package-to-install>`

## Your first program!

Ideally this will be enough to get you started.

Open VSCode. You can then open the terminal by pressing.

```
Cmd+` (the backquot\backtick is usually on your Esc key)
```

This will hopefully be the only way you interact with the terminal. 

Type in the terminal:

```
git init # not neccesary if you don't have git
pipenv shell # not neccesary if you don't have pipenv
pip install pybedtools
```

Then you can write a program that opens your bed file and prints out all the sequences:

```python
from pybedtools import BedTool
genes = BedTool('bed_file.bed')

for gene in genes:
  print(gene)
```

If you get stuck: https://www.pythoncheatsheet.org/

If you get the simple bedfile running then you will need more stuff to work on. I recommend you start looking at https://github.com/ossu/bioinformatics
 for more information on what you need to do. I can always help with a problem if it is needed.

## Python Practice, practice, practice!

https://exercism.io/tracks/python

That website has a good list of challenges. It will help you get better with python over time and it is what I use.

It won't help you become a super star in python overnight, but doing 30 minutes a day can help tremendously in the long run.

## Bioinformatics

### Useful python packages

Data analysis is important so here is a list of useful packages:
 - https://github.com/vinta/awesome-python#data-analysis

Pandas is a python library that is the same to R's dataframes. So it is neccesary to easily onboard users from R to Python:

Install by running this command in the terminal:

```
pip install pandas
```

## More advanced topics and for you to get started on your own

 - https://github.com/danielecook/Awesome-Bioinformatics
 - https://github.com/ossu/bioinformatics
 - https://github.com/jtoy/awesome-tensorflow
 - https://github.com/chapmanb/bcbb
 - https://github.com/HussainAther/awesome-alternative-splicing

## Books 

I have these books and I can share them with you:

 - Dive Into Python 3 - Mark Pilgrim.pdf
 - Python 201 - Michael Driscoll.pdf
 - Bayesian Analysis With Python.pdf
 - Picking A Python Version-A Manifesto.pdf
 - Learning Data Mining with Python.pdf
 - Python Programming For The Absolute Beginner-Third Edition.pdf
 - Head First Python.pdf
 - Python Machine Learning By Example.pdf
 - Python Machine Learning Cookbook.pdf
 - Python Data Visualization Cookbook.pdf
 - Doing Math With Python.pdf
 - 20 Python Libraries You Aren'T Using But Should.pdf
 - How To Make Mistakes In Python.pdf
 - Python Pocket Reference-5th Edition.pdf
 - Scientific Computing with Python 3.pdf
 - Python Machine Learning Blueprints.pdf
 - Mastering Python.pdf
 - Beginner'S Python Cheat Sheet.pdf
 - Introduction To Programming Using Python.pdf
 - Learn Python The Hard Way-Third Edition.pdf
 - Learning Python.pdf


## TODO

[ ] Add a better introduction to the terminal
