# How to install php with Choco

## Checking

```bash
Prawee@THRL-11154 MINGW64 ~
$ choco search php
```

```bash
Chocolatey v0.10.15
php 7.4.3 [Approved]
...
```

```bash
$ php -v
bash: php: command not found
```

## Install

```bash
$ choco install php
```

```bash
Environment Vars (like PATH) have changed. Close/reopen your shell to
 see the changes (or in powershell/cmd.exe just type `refreshenv`).
 The install of php was successful.
  Software installed to 'C:\tools\php74'
```

## Version

After install close `CMD` first and open again
