# MathSupCode
A MathSupCode repo to automate calculs. College level.

# Contents 
- [Features](#features)
- [Usage](#usage)
- [Build](#build)
- [Issues](#Issues)
<Documentaion>

# Features
MathSupCode contains just some features for moment.
There is from far only one speciality.

##  Analysis
Analysis is the branch of mathematics dealing with continuous functions, limits, and related theories, such as differentiation, integration, measure, infinite sequences, series, and analytic functions. 

### Functions :
- A function to say if a number is rationnal or no.
    > analyse.is_rationnal()
- A function to change the form of a rationnal number.
    > analyse.change_form()

# Usage 
To use MathSupCode we can for moment clone the repo and use it as python library.

# Build 
To build the python environment for MathSupCode, we have to clone the repo: \
`git clone https://github.com/thamnis/MathSup.git` or 
`git clone git@github.com:thamnis/MathSup.git`

Then, you can use and enjoy MathSupCode.

# Issues 
If you get some issues while building or using MathSupCode, this is opensource, so you can ensure the issue and commit. All issues news will be added here. At this moment, this is some issues reported : 

### 1. Visual Studio Code "module not found" error
If you get this problem, you can correct it by some manipulations.
1. Create a _.vscode_ directory if not existing and create two files : _launch.json_ and _settings.json_. or execute :
###  If in Linux or MacOS
    mkdir ".vscode" && touch "launch.json" "settings.json"
###  In Windows 
    mkdir ".vscode" ; echo $null >> filename

Then, copy the following content in differents files:

- launch.json

> {
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Module",
            "type": "python",
            "request": "launch",
            "module": "main.py",
            "env": {"PYTHONPATH": "${workspaceFolder}/libs"}
        }
    ]
}

- settings.json
> {
    "python.analysis.extraPaths": ["${workspaceFolder}/libs/"]
}

# Credits
- Author : [thamnis](https://github.com/thamnis)
- Creation date : 2024-10-27
- Licence : [MIT Licence](LICENSE)

<Have to be enhanced>