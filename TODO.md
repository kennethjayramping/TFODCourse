Before doing anything else, click CTRL + SHIFT + P, then click Open Workspace Settings. Add in this code,

"terminal.integrated.profiles.windows": {
  "PowerShell": {
    "source": "PowerShell",
    "icon": "terminal-powershell",
    "args": ["-ExecutionPolicy", "Bypass"]
  }
},
"terminal.integrated.defaultProfile.windows": "PowerShell",

then click Save. Restart VS Code, close all terminals and start a new terminal by hitting the + sign.