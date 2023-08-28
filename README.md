# Typosquatting checker

Package typosquatting is a type of software supply chain attack where the attacker tries to mimic the name of an existing package

This is Typosquatting detection tool (part of Supply Chain Security) for Python (PyPi) packages is designed to prevent this attack. 

This tool checks typos for the PyPi [list of popular packages](https://hugovk.github.io/top-pypi-packages/).

## Getting started

Follow these steps to get started with Typosquatting Checker:

### Installation

1. Install the necessary libraries using the following command:

    ```
    pip3 install -r requirements.txt
    ```

### Usage

1. Start 'typoschecker' for test a requirements_test.txt file:

   ```
   python3 typoschecker.py test_requirements/requirements_test.txt 
   ```
   If any potential typosquatting packages are detected, the tool will provide suggestions for possible correct package names.
   
   Results:
   ![example.png](test_requirements%2Fexample.png)

2. Update the PyPi list of popular packages:

   ```
   python3 typoschecker.py --update 
   ```
   
3. Get help on usage:

    ```
    python3 typoschecker.py --help
    ```
4. Use case:
