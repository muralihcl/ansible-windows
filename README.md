## This repository contains the PowerShell scripts to enable PS Remoting on Windows for ansible to interact with Windows using WinRM

Courtesy: https://github.com/AlbanAndrieu/ansible-windows

To use this script, make sure to launch PowerShell with admin privileges.

```powershell
cd C:\
$url = https://raw.githubusercontent.com/muralihcl/ansible-windows/master/scripts/ConfigureRemotingForAnsible.ps1
$destination = "C:\ConfigureRemotingForAnsible.ps1"
Invoke-WebRequest $url -OutFile $destination
.\ConfigureRemotingForAnsible.ps1
```

This will complete necessary configuration of the Windows PowerShell remoting feature to help it integrate with Ansible.
