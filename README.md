# vagrant-safe-linux

Vagrant environment for Safe Linux Proof-of-Concept.

### Prerequisites

* A recent PC with a 64-bit OS capable to run VirtualBox and Vagrant (tested on a Dell Precision 5510 with MS Windows 10)
* A fast Internet connection
* [Oracle VM VirtualBox](https://www.virtualbox.org/) v5.1.22 or later
* [Vagrant](https://www.vagrantup.com/) v1.9.5 or later

### Step-by-step instructions

Make sure you have all the prerequisite met, then check-out the git repository and type the following commands

```
vagrant box update
vagrant up
```

NOTE: This command may take a few minutes to complete until all the VMs have been created and booted successfully.

You may verify that all the guest VMs are running with the `vagrant status` command:

```
vgmacario@ITM-GPAOLO-W10:~/MYGIT/gmacario/vagrant-safe-linux $ vagrant status
Current machine states:

ch1                       running (virtualbox)
ch2                       running (virtualbox)

This environment represents multiple VMs. The VMs are all listed
above with their current state. For more information about a specific
VM, run `vagrant status NAME`.
gmacario@ITM-GPAOLO-W10:~/MYGIT/gmacario/vagrant-safe-linux $
```

You may then log into each of the computing channels with the following command

```
vagrant ssh ch1
```

or

```
vagrant ssh ch2
```

To stop the VMs type the following command

```
vagrant halt
```

To destroy the VMs type the following command

```
vagrant destroy
```

### Copyright and License

vagrant-safe-linux is an Open Source program - for details please see the `LICENSE` file.

Copyright (C) 2017, [Gianpaolo Macario](https://gmacario.github.io/).

<!-- EOF -->
