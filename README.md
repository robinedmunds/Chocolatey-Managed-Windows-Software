# Chocolatey Managed Windows Software

Running `choco-install-all.ps1` in PowerShell will install all software packages in the list from the chocolatey community package index. All these software packages are then managed by the Chocolatey package manager for easy updating.

## First run

1. [Install chocolatey](https://chocolatey.org/install)
1. Open elevated PowerShell shell (Ctrl-Shift click)
1. Run `./choco-install-all.ps1`

## Updating packages

1. Open elevated PowerShell shell (Ctrl-Shift click)
1. Run `choco outdated` to get list of outdated packages
1. Run `choco upgrade --yes all` to upgrade all outdated packages

## List installed packages

1. `choco list | Select-String regex`

## Version pinning

```powershell
choco pin
choco pin list
choco pin add -n git
choco pin add --name="'git'" --version="'1.2.3'"
choco pin add --name="'git'" --version="'1.2.3'" --reason="'reasons available in business editions only'"
choco pin remove --name="'git'"
```

## Remove packages

```powershell
choco uninstall git
choco uninstall notepadplusplus googlechrome atom 7zip
choco uninstall notepadplusplus googlechrome atom 7zip -dv
choco uninstall ruby --version 1.8.7.37402
choco uninstall nodejs.install --all-versions
```



[Chocolatey command reference](https://chocolatey.org/docs/commands-reference)
