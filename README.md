# Simple GitHub Auto Saver - SGHAS -
A simple bat file to backup your project periodically into GitHub in case things goes south

<h3>Disclaimer</h3>
First of all, its recommended for you to have the basic knowledge of git in order to set it up
And since its a simple .bat file, feel free to edit it the way it fits better for you, ive only set the basic to make it work without much set up.

<h2>First Steps</h2>

1 - Install git<br>
2 - Install Winrar<br>
3 - Create your repo on Github (if you dont have one already)<br>
4 - Download the GitUpdater.bat file above<br>

<h2>How to set up</h2>

1 - Clone your Repository localy<br>
2 - Right click the .bat file, on the first few lines you should see:<br>

set BackupDir=<br>
set WINRAR=<br>
set PASSWORD=<br>

Here, you will paste the directory of the repository you want to back up, the Winrar executable path, and the password to decompress your backup, and save it, Example:<br>

set BackupDir=C:\MyBackupFolder<br>
set WINRAR=C:\Program Files\WinRAR\Rar.exe<br>
set PASSWORD=YouJustLostTheGame<br>

By default, the Backup will be stored with the repository itself, on its main branch, but you can change it to wherever you wanna save it bellow on the line "git push origin main"
(My recomendation would be to toss it into a separate branch or just create a secondary repo to store it, but since im trying to keep it basic, again, change it to however you like it)

Now you got 2 options
1 - Press Win + R and type shell:startup, toss the .bat there, and if you done everything correctly, each time you boot your pc it should run itself and backup everything
2- Use Windows Task Schedule to run it in fixed periods of time
