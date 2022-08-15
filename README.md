## AstOS (Arch Snapshot Tree OS)

![astos-logo](logo.png)

AstOS is a modern distribution based on [Arch Linux](https://archlinux.org).  
Unlike Arch it uses an immutable (read-only) root filesystem.  
Software is installed and configured into individual snapshot trees, which can then be deployed and booted into.  
It doesn't use it's own package format or package manager, instead relying on [pacman](https://wiki.archlinux.org/title/pacman) from Arch.

## AstOS compared to other similar distributions
* **NixOS** - compared to nixOS, AstOS is a more traditional system with how it's setup and maintained. While nixOS is entirely configured using the Nix programming language, AstOS uses Arch's pacman package manager. AstOS consumes less storage, and configuring your system is faster and easier (less reproducible however), it also gives you more customization options. AstOS is FHS compliant, ensuring proper software compatability.
  * AstOS allows declarative configuration using Ansible, for somewhat similar functionality to NixOS
* **Fedora Silverblue/Kinoite** - AstOS is more customizable, but does require more manual setup. AstOS supports dual boot, unlike Silverblue.
* **OpenSUSE MicroOS** - AstOS is a more customizable system, but once again requires a bit more manual setup. MicroOS works similarly in the way it utilizes btrfs snapshots. AstOS has an official KDE install, but also supports other desktop environments, while MicroOS only properly supports Gnome. astOS supports dual boot.


This is a sneak-peek at Astos tree structure. One can have all these in one computer in an immutable way:
- An absolutely bare minimum base
- A Gnome desktop with touch/tablet drivers installed
- A Gnome desktop with TKG kernel for gaming with Nvidia drivers
- An instance with Sway windows manager

```
├── 0 - base image
└── 1 - multiuser system
    └── 4 - applications
        ├── 6 - MATE full desktop
        └── 2*- Plasma full desktop
```

# More Information
There is a lot more to Astos. Please take a look at [official repository](https://github.com/astos/astos) to get more acquainted with Astos!

# Community
* Please feel free to join us on [Discord](https://discord.gg/YVHEC6XNZw) for further discussion and support!
* Happy worry-free snapshotting!
