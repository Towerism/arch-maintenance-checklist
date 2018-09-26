# arch-maintenance-checklist
> Checklist for maintaining arch linux system

## Upgrading system

- Check https://www.archlinux.org for package news
- Perform `pacman -Syu`
- Check AUR if there any upgrades `yay -Qua`
- Perform `yay -Syu`
- Check for orphaned packages `pacman -Qtd` (packages which are no longer
  depended on)
- Remove those packages with `pacman -Rns $(pacman -Qtdq)`
- Check manually installed packages (AUR helper) `pacman -Qm`
- Remove any which you deem unnecessary at this point in time

