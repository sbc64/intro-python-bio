# Intro to python bio

This document assumes you have no experience with python or the commandline and will hopefully get you up to speed. If you want to just use 

## Why python?

Why python and not R? I think they are both great! They have incredibly strong support in bioinformatics. The only advantage I see with python is that you can use it for other programming areas that R might not be as good at. Python also has a stronger Machine Learning support.

## Github
The first step is to make a github account: https://github.com/join?source=header-home

And then follow some bioinformatitians:
https://github.com/BenLangmead
https://github.com/johanneskoester
https://github.com/dcjones
https://github.com/sjackman

Following people allows you to  discover what they like and you might something interestin.

You should also download https://desktop.github.com/

## Programming environment

### IDE (Integrated development environment)

Install https://code.visualstudio.com/

Why VScode? It is the most simple IDE but at the same time it is the most powerful when extensions get added. Other IDEs have way too many buttons and you can easily get lost. In the end you can learn how to use python with just a commandline and a text file. But we don't want to be that extreme.

### Python3.

Just use python 3 everywhere. Avoid python2
Install: https://docs.python-guide.org/starting/install3/osx/

### Pipenv

Pipenv is a tool to make each project you work on have different libraries python libraries. Sometimes you can have two libraries. Say csv-parser and csv-parser-3000 and they both use a different common library called dictionary-handler-2000. If you install both csv libraries at the system level they will both be stepping over each installing the different versions of disctionary-handler-2000. It is not strictly neccesary but I highly recommend it. You can start


## Your first program!

Open VSCode. You can then open the terminal by pressing.

```
Cmd+` (the backquot\backtick is usually on your Esc key)
```

Type in the terminal:

```
git init
pipenv shell
```

## Practice, practice, practice!

https://exercism.io/tracks/python

That website has a good list of challanges. It will help you get better with python over time and it is what I use.

## More advanced topics and for you to get started on your own

https://github.com/danielecook/Awesome-Bioinformatics
https://github.com/ossu/bioinformatics

### ML
https://github.com/jtoy/awesome-tensorflow


If you want any book just tell me and I can probably get it for you.
