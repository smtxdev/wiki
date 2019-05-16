# Setup Docker

## Docker for Mac (for newer Macs)

### Requirements

- Mac hardware must be a 2010 or newer model, with Intel’s hardware support for memory management unit (MMU) virtualization, including Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: sysctl kern.hv_support
- Mac hardware must be a 2010 or newer model, with Intel’s hardware support for memory management unit (MMU) virtualization, including Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: `sysctl kern.hv_support`
- At least 4GB of RAM
- VirtualBox prior to version 4.3.30 must NOT be installed (it is incompatible with Docker Desktop for Mac). If you have a newer version of VirtualBox installed, it’s fine.

### Install

- `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
- `brew cask install docker`
- Command + Space to bring up the spotlight search and enter `Docker` to launch Docker.
- Follow the wizard and confirm with `yes`/`ok` the prompts. You might need to enter your password.
- `brew install docker-compose`
- `sudo chmod 666 /etc/hosts`

## Docker for Windows (for newer Windows-Systems)

### Requirements

- Windows 10 64bit: Pro, Enterprise or Education (Build 15063 or later).
- Virtualization is enabled in BIOS. Typically, virtualization is enabled by default. This is different from having Hyper-V enabled. For more detail see Virtualization must be enabled in Troubleshooting.
- CPU SLAT-capable feature.
- At least 4GB of RAM.

### Install

- Open an administrative shell: `cmd` or `powershell`.
- cmd: `@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
- powershell: `Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`
- `choco install docker-desktop`


## Docker Toolbox (for older Macs)

### Install

- `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
- `brew cask install docker-toolbox`
- `sudo chmod 666 /etc/hosts`


## Docker Toolbox (for older Windows-Systems)

### Install

- Open an administrative shell: `cmd` or `powershell`.
- cmd: `@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
- powershell: `Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`
- `choco install docker-toolbox`
