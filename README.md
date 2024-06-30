# How to use USpekPy?

Welcome to the USpekPy tutorial! USpekPy is a tool designed to simplify the computation of integral quantities for x-ray spectra with uncertainties. 
This tutorial will guide you through the installation process and provide practical examples to help you make the most of its features. 
By the end of this tutorial, you'll be equipped with the knowledge to effectively use USpekPy for your x-ray spectrum analysis needs.

This tutorial is prepared to be followed using the PyCharm IDE. 
However, the steps are basically the same if you are using another IDE.

## Table of Contents
- [How to install USpekPy?](#how-to-install-uspekpy)
- [Examples of USpekPy usage](#examples-of-uspekpy-usage)

## How to install USpekPy?
Welcome to the installation guide for USpekPy! 
In this section, we will walk you through the steps to set up USpekPy on your computer using PyCharm IDE. 
Whether you're a beginner or an experienced user, this guide will help you get USpekPy up and running smoothly.

This is the summary of the steps to install USpekPy using PyCharm IDE:
1. Clone the seminar repository to your computer
2. Set up a virtual environment for the project
3. Install uspekpy
4. Fix SciPy dependency issue

Before starting, make sure you have [Python 3.8](https://phoenixnap.com/kb/upgrade-python) or superior and 
[PyCharm](https://www.jetbrains.com/help/pycharm/installation-guide.html) installed on your computer. Let's go!

1. **Clone the seminar repository to your computer:**
  - Click on `Get from VCS` on the PyCharm welcome screen.
  - In the `Get from Version Control` dialog:
  - In the `Get from Version Control` dialog, you can select which version control system to use in the `Version control` dropdown menu. This example will use Git.
  - In the `URL` field, paste the URL to the `uspekpy-seminar` repository at GitHub. The repository URL is `https://github.com/xandratxan/uspekpy-seminar.git`. To find the repository URL:
    - On `GitHub.com`, navigate to the main page of the repository.
    - Above the list of files, click `Code`.
    - Copy the URL for the repository clicking the copy symbol to the right.
  - In the `Diretory` field, select the directory to clone the project.
  - Click `Clone`.

    Note: This repository is for educational purposes only. You will not be able to push changes into it.
   
2. **Set up a virtual environment for the project:**
  - In PyCharm, go to `File > Settings`.
  - Navigate to `Project: uspekpy-seminar > Python Interpreter`.
  - Click on `Add interpreter` next to the current interpreter and select `Add Local Interpreter...`.
  - In the "Add Python Interpreter" dialog, select `Virtualen Environment` in the right panel.
  - In the "Environment" field, select "New". By default, Pycharm creates a directory called "venv" under your project root directory.
  - Then click "Ok"
  - Back in the "Settings" dialog, ensure that the newly created virtual environment is selected as the project interpreter.
  - Then click "Apply" and "Ok"
  - Check that the virtual environment is active:
    - In the right toolbar of Pycharm, click the `Terminal` icon to open the system terminal tool window.
    - Click the `New tab` icon to open a new terminal.
    - You should see `(venv)` in the terminal prompt.

3. **Install uspekpy**
- In the right toolbar of Pycharm, click the `Python Packages` icon to open the package manager tool window.
- In the search tool, type "uspekpy". Under the `PyPI` tab of the results you should see `uspekpy`.
- Click the `Install package` button to the right of the tool window to install the latest version of USpekPy.
 
4. **Fix SciPy dependency issue:** 
When you install USpekPy, the latest stable version of SciPy (1.14.0) is installed as a dependency.
However, there is an active issue regarding the SciPy version, and USpekPy will not run with this version of SciPy.
To work around this issue until it is fixed, yu can do the follow the next steps:
- In the right toolbar of Pycharm, click the `Python Packages` icon to open the package manager tool window.
- In the search tool, type "scipy". Under the `Installed` tab of the results you should see `scipy 1.14.0`.
- Click the three dotted icon to the right of the tool window and select `Delete Package` to uninstall the latest version of SciPy.
- Once uninstalled, click `latest` on the right of the tool window and select the version 1.13.1.
- Click the `Install package` button to the right of the tool window to install the version 1.13.1 of SciPy.

Now you are ready to go!

## Examples of USpekPy usage
Now that you have USpekPy installed, it's time to explore its capabilities! 
This section provides practical examples of how to use USpekPy to compute integral quantities for x-ray spectra. 
These examples will guide you through different use cases, from simple single-case computations to handling multiple cases using various input files.

Using USpekPy to compute integral quantities for x-ray spectra:
1. Values for a single case
2. Values for a single case using data files
3. Values and uncertainties for a single case
4. Values and uncertainties for a single case using data files
5. Values and uncertainties for several cases using CSV input file
6. Values and uncertainties for several cases using Excel input file
