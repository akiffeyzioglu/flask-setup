## Flask & Vagrant Local Development Environment

## Table of Contents

* [How to Use Python Virtual Environment](#how-to-use-python-virtual-environment)

## How to use Python Virtual Environment

Go to your development directory and run: 
```
pip install virtualenv
```
Create virtual environment: 
```
virtualenv venv
```
For MacOS and Linux:
```
source venv/bin/activate
```
Windows:
```
venv\Scripts\activate
```
Install dependencies:
```
pip install -r requirements.txt
```
Deactivate virtual environment:
```
deactivate
```