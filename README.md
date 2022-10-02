## AshOS (Any Snapshot Hierarchical OS)

![ashos-logo](logo.png)

You always wanted to try Fedora Rawhide but after a few days, its fragility got on your nerves. Then, maybe you tried Fedora Silverblue Rawhide but then its complicated and slow git-like ostree operations killed your mood! Well, no more! Now you can try this bleeding edge distro (and many more distros like Debian sid) with more peace of mind.

AshOS is a unique meta-distribution that aims to bring immutability even to distros that do not have this very useful feature i.e. Arch Linux, Gentoo, etc. Software is installed and configured into individual snapshot trees, which can then be deployed and booted into.

This is a sneak-peek at AshOS tree structure. One can have all these in one computer in an immutable way:
- An absolutely bare minimum base
- A Gnome desktop with touch/tablet drivers installed
- A Gnome desktop with TKG kernel for gaming with Nvidia drivers
- An instance with Sway windows manager
- And much more

```
├── 0 - base image
└── 1 - multiuser system
    └── 4 - applications
        ├── 6 - MATE full desktop
        └── 2*- Plasma full desktop
```

# More Information
There is a lot more to learn about AshOS (for instance how it compares to NixOS, Fedora Silverblue/Kinoite, OpenSUSE MicroOS, etc.). Please take a look at README at [AshOS official repository](https://github.com/ashos/ashos)!

# Community
* Feel free to join us on [Discord](https://discord.gg/YVHEC6XNZw) for further discussion and support!
* Subscribe to our [YouTube channel](https://youtube.com/channel/UCj1U5kmpGGvUrbaZtMsorkw) for more hands-on demos and walk-throughs for installation
* Happy worry-free snapshotting!

