# How to search and installation NodeJS

## Checking

```bash
$ node -v
bash: node: command not found
```

```bash
$ npm -v
bash: npm: command not found
```

## Search

```bash
$ choco search nodejs
```

```bash
Chocolatey v0.10.15
nodejs 13.12.0 [Approved]
...
30 packages found.
```

## Install

```bash
$ choco install nodejs
```

```bash
Chocolatey v0.10.15
Installing the following packages:
nodejs
By installing you accept licenses for the packages.
Progress: Downloading nodejs.install 13.12.0... 100%
Progress: Downloading nodejs 13.12.0... 100%

nodejs.install v13.12.0 [Approved]
nodejs.install package files install completed. Performing other installation steps.
The package nodejs.install wants to run 'chocolateyInstall.ps1'.
Note: If you don't run this script, the installation will fail.
Note: To confirm automatically next time, use '-y' or consider:
choco feature enable -n allowGlobalConfirmation
Do you want to run the script?([Y]es/[A]ll - yes to all/[N]o/[P]rint): Y
```

```bash
Installing 64 bit version
Installing nodejs.install...
nodejs.install has been installed.
  nodejs.install may be able to be automatically uninstalled.
Environment Vars (like PATH) have changed. Close/reopen your shell to
 see the changes (or in powershell/cmd.exe just type `refreshenv`).
 The install of nodejs.install was successful.
  Software installed as 'msi', install location is likely default.

nodejs v13.12.0 [Approved]
nodejs package files install completed. Performing other installation steps.
 The install of nodejs was successful.
  Software install location not explicitly set, could be in package or
  default install location if installer.

Chocolatey installed 2/2 packages.
 See the log for details (C:\ProgramData\chocolatey\logs\chocolatey.log).
```

```bash
$ exit
```

```bash
$ node -v
v13.12.0
```

```bash
$ nmp -v
6.14.4
```

```bash
$ npx -v
6.14.4
```
