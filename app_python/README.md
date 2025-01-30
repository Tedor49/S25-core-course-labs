# Web application to display current time in Moscow

## Overview

This application uses Python, Flask and Waitress to host a web page to shown
the current time in Moscow. The app serves a single webpage, which contains
the current time and date in Moscow, along with some minimalistic 
formatting. You can find the source code in [app.py](app.py), the [HTML](resources/templates)
and [CSS](resources/static) files in [resources](resources). Required python packages are in
[requirements.txt](requirements.txt) and some implementation justifications are in [README.md](README.md)

## Setup

### Python

Download Python 3 from [the official website](https://www.python.org/downloads/) and make sure to add it to PATH.

Install pip from command line if it is not already installed:
```
python -m ensurepip --upgrade
```

### Requirements

From the command line, inside the repository directory, run
```
pip install -r requirements.txt
```

### Running the web application

From the command line, inside the repository directory, run
```
waitress-serve --host your_ip --port your_port "app:app"
```
your_ip and your_port have to be replaced by the ip you wish to host on
and the port number respectively, for example: 
```
waitress-serve --host 127.0.0.1 --port 8080 "app:app"
```
After hosting, you can connect to the web app from any browser using 
the provided ip and port, which will also be shown in the terminal.

