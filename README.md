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