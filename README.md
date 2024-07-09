# AutomaticLolPatchNotes
Automatically checks if new patch notes are up and then opens them.

Can be put into autostart to check new patch notes every bootup.

> `Win+R` -> Type: "shell:startup" -> Move the `start_lolnewsopener.bat` into the Windows-Autostart-Directory

Open the bat-file and change the directory to the LolNewsOpener.py in your autostart

# Setup
1. Download the Repository
2. Start the `setup.bat` to install  all pip install `requirements.txt` for the use of this script
3. If you haven't installed python3 yet, do so as it needs to run a python script
4. Remotely start the batch or move it into autostart as mentioned above
5. Enjoy!


# Troubleshooting
- **Read any exceptions by adding 'pause' as last statement in the `start_lolnewsopener.bat`**
    - Edit the ``start.bat`` to look like this to read any exceptions that had been thrown:
```
@echo off
cd [PROGRAMS DIRECTORY e.g. C:/PythonPrograms/AutomaticLolPatchNotes] 
python.exe LolNewsOpener.py
pause
```


