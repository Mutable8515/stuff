# stuff
just overflow stuff. May or may not add things over time. Due to laziness I'm using it as a share for now. Main repo is self-hosted and a chore to open things up outside my tailnet.

## apps
- app launcher and arch package manager script
  - ctrl+s puts in install mode to search core, extra, aur, and flathub for installation
  - ctrl+x puts in remove mode to search install apps and uninstall them
  - ctrl+r puts in launcher mode (default) to launch gui apps on system. works like typical launchers but in terminal and without icons
 
 ## updatecount
 - updatecount script for checking for system updates and outputting a single integer for the count
   - Arch focused. Requires yay or paru and pacman-contrib package for checkupdate command (more reliable for getting repo update counts)
   - Also checks flatpak/flathub for available updates on the system
   - Single integer output aggregates all the sources and works especially well for something like the update-count plugin in noctalia-shell

  ## update 
  - update is a simple update script that pairs well with update count
    - lists the apps to be updated before asking to proceed (rather than just launching into an update, so you can abort before all the noise shows up).
    - Only lists from sources with updates. So if only AUR updates, you won't see empty lists for pacman and flatpak. You will see just the AUR list. Not major, but neater.
