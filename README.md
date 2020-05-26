# fsCapture.py
Field Strength Capture - Python script to capture measurements from Rohde and Schwarz ETL analyzer

To run this script, launch it from a CMD prompt or from a Desktop
Shortcut with a command like this:

>  python C:\Shared\batch_files\fsCapture.py

## REQUIREMENTS 
This script requires Python version 3.x, which can be downloaded
from python.org. It also requires modules, which can be installed
by issuing this at the CMD prompt:

>  pip3 install openpyxl pyvisa pyvisa-py ntplib

## INI FILE 
The script stores variables in an INI file:

>  `%APPDATA%\Osborn\fsCapture.INI`

This file can be viewed and/or edited with NOTEPAD, although this
should not be necessary.

An alternate INI file can be specified as the second argument on 
the command line:

>  `python \shared\batch_files\fsCaptureDEV.py info Z:\fsCapture.INI`

This script specifies paths in the Windows operating system. To
run under linux or Mac, launch with an alternate location for the 
INI file, like this example:

>  `python3 /path/to/fsCapture.py info /home/user/fsCapture.ini`

## LOGS
The script writes logs of its activities in the same directory
as the INI file.

To increase the detail of the logging, call the script
with "debug" as the first argument, like this:

>  `python C:\Shared\batch_files\fsCapture.py debug`
