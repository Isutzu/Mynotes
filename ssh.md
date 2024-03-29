# SSH

With SSH we can connect to the server terminal, issue commands, install programs, make configurations just like we were sitting in front of the server terminal.

**ssh-keygen** Creates _id\_rsa_ and _id\_rsa.pub_ files in the .ssh directory the which contain the private and public key respectively. Private key should never be shared to avoid a men in the middle attack.

**known\_hosts** file is located in the client(local) machine and contains the list of public keys of the servers we have connected to.

**authorized\_keys** file is located in the server(remote) machine and contains the public keys of the clients that have stablished a connection

**Connecting to Server without password** Copy the public key _id\_rsa.pub_ in the authorized\_keys file of the remote server. If the file does not exists just create it.([Video demo - learnCode.academy](https://youtu.be/DbPDraCYju8))

_Resources:_

* [setting ssh passphrases](https://help.github.com/articles/working-with-ssh-key-passphrases/)
* [ssh config file](https://mediatemple.net/community/products/grid/204644730/using-an-ssh-config-file)
* [create an additional known host entry](https://superuser.com/questions/416246/generating-known-host-entry)
* [known\_hosts and authorized\_keys](https://unix.stackexchange.com/questions/42643/ssh-key-based-authentication-known-hosts-vs-authorized-keys)
* [difference between known\_hosts and authorized\_keys](https://security.stackexchange.com/questions/20706/what-is-the-difference-between-authorized-keys-and-known-hosts-file-for-ssh)
* [Understanding the SSH Encryption and Connection Process](https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process#how-does-ssh-work)

## Bash prompt customization

on Mac open the .bash\_profile in the home directory and add the PS1 shell variable. PS1 variable controls the prompt and it is configured before accepting any commands.([video demo from Corey Schafer ](https://youtu.be/LXgXV7YmSiU)).

## Xcode

it is a package that contains Apple developer tools.It also contains the gcc compiler which allows to prepare open source software to use in our computer. For example, when installing Ruby we will need the gcc compiler to be installed

**homebrew** open software for managing open software on mac.

## UNIX symbolic & hard links

A hard link points to the same file from a different location. and different name.

Use symbolic links to make a shortcut to a long directory path

`ln -s /path/to/file /path/to/link`

_Resources:_

[symbolic and hard links](https://www.lifewire.com/create-symbolic-links-ln-command-4059723)

[what are symbolic and hard links](https://www.lifewire.com/what-are-hard-links-2190041) \


## Shorcut keys

`cmd+k` :clear screen.

#### Links

[_Shell Programming in Unix, Linux and OS X, 4th edition_ by Kochan and Wood](https://www.pearson.com/us/higher-education/program/Kochan-Shell-Programming-in-Unix-Linux-and-OS-X-The-Fourth-Edition-of-Unix-Shell-Programming-4th-Edition/PGM334337.html).
