# AntlrWindowsExample
### if you dont like to read...
>Guide i used: https://www.youtube.com/watch?v=p2gIBPz69DM

## Dependencies
Download [Complete ANTLR 4.11.1 java binaries jar](https://www.antlr.org/download/antlr-4.11.1-complete.jar "LINK FOR COMPLETE ANTLR jar")
set a %CLASSPATH% in your env variables.
### Windows-specific issues

On Windows, the `pip` command doesn't just work---you need to add the `...\local-packages\python38\scripts` dir to your `PATH`, which itself might require a fun reboot.  If you use WSL on Windows, then the pip install will also properly at the scripts directly (if you run from bash shell).


1. Go to the Microsoft Store
2. Search in Microsoft Store for Python
3. Select the newest version of Python (3.10).
4. Click the "Get" button. Store installs python and pip at "c:\Users...\AppData\Local\Microsoft\WindowsApps\python.exe" and "c:\Users...\AppData\Local\Microsoft\WindowsApps\pip.exe", respectively. And, it updates the search path immediately with the install.
5. Open a "cmd" terminal.
6. You can now type "python" and "pip", and "pip install antlr4-tools". 7. Unfortunately, it does not add that to the search path.
7. Update the search path to contain `c:\Users...\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p8\LocalCache\local-packages\Python310\Scripts`. You may need to install MSYS2, then do a `find /c/ -name antlr4.exe 2> /dev/null` and enter that path.
8. Or, you can set up an alias to antlr4.exe on that path.

The good news is that the ANTLR4 Python tool downloads the ANTLR jar in a standard location, and you don't need to do that manually. It's also possible to go in a browser, go to python.org, and download the python package. But, it's likely you will need to update the path for antlr4.exe as before.

## How to run. Commands:
### In example folder run this commands

>class

>antlr experiment.g4

>javac experiment*.java

>grun experiment start example.txt -gui

### Still having trouble?
>Guide i used: https://www.youtube.com/watch?v=p2gIBPz69DM

# RESULT

# ![image](https://user-images.githubusercontent.com/107003088/190939526-1d7a1039-ca16-4994-b0be-9c22517c9b58.png)



