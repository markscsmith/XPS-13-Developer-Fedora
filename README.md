# XPS-13-Developer-Fedora
This is a basic Ansible playbook to set up Fedora 25 the way I like on my laptop.

I'm using it on my XPS 13 Developer Edition (9360)

What changes does this playbook make?

Two things:
* Change CapsLock into a third Ctrl key for ergonomic reasons using udev rules.
* Set the trackpad to remain active while typing using Xorg and libinput settings.

To run:

    $ dnf install ansible
    $ ansible-playbook keyboard.yaml
    
Information sources:

[Arch Wiki](https://wiki.archlinux.org/index.php/Map_scancodes_to_keycodes): CapsLock -> Ctrl 
* indrect info: examples use other mappings



[openSUSE Forum](https://forums.opensuse.org/showthread.php/521887-turn-off-disable-touchpad-while-typing?p=2805461#post2805461): Enable the trackpad while typing 
* indrect info: post gives instructions to *disable* the trackpad while typing

