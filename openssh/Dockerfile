# escape=`

# Basic Windows Server 2019 image 
FROM mcr.microsoft.com/windows/servercore:ltsc2019


RUN powershell -NoProfile -NoLogo -Command `
    Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0 ; `
    Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0; `
    Start-Service sshd; `
    Set-Service -Name sshd -StartupType 'Automatic'; `
    Get-NetFirewallRule -Name *ssh* ; 

# Default to PowerShell if no other command specified.
CMD ["powershell.exe", "-NoLogo", "-ExecutionPolicy", "Bypass"]


