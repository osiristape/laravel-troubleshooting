## npm : File C:\laragon\bin\nodejs\node-v18\node_modules\npm\bin\npm.ps1 cannot be loaded because running scripts is disabled on this system.
- open powershell as administrator
- "Get-ExecutionPolicy" copy and paste to terminal
- "Set-ExecutionPolicy Unrestricted" then, 'npm run dev'


always makes sure the environment variable set as 'C:\Program Files\nodejs' for readability of resources (nodejs)
- NVM_HOME = "C:\Users\MyComputer\AppData\Roaming\nvm"
- NVM_SYMLINK = "C:\Program Files\nodejs" 

![](https://github.com/osiristape/laravel-troubleshooting/blob/main/image.png)
