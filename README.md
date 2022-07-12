# Chocolatey Managed Windows Software

Running `choco-install-all.ps1` in PowerShell will install all software packages in the list from the chocolatey community package index. All these software packages are then managed by the Chocolatey package manager for easy updating.

## First run

1. [Install chocolatey](https://chocolatey.org/install)
1. Open elevated PowerShell shell (Ctrl-Shift click)
1. Run `./choco-install-all.ps1`

## Updating packages

1. Open elevated PowerShell shell (Ctrl-Shift click)
1. Run `choco outdated` to get list of outdated packages
1. Run `choco upgrade all --yes` to upgrade all outdated packages

## List installed packages

1. `choco list --local-only`

[Chocolatey command reference](https://chocolatey.org/docs/commands-reference)
