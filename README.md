# Poor man's reboot-required
Creates a reboot-required file under /var/run if one of the packages specified in _pmrr.conf_ is updated on an Arch Linux system via pacman. Removes it on reboot if the _pmrr-reboot-required.service_ is activated.

Add the packages that should trigger the creation of the file in _/etc/pmrr.conf_. Run _pmrr-regenerate-hook_ to regenerate the hook for the changes to take effect.
