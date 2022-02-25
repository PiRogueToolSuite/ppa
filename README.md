# PiRogue Debian packages

To install PiRogue packages, execute the following command in a terminal:

```bash
sudo curl -o /etc/apt/sources.list.d/pirogue.list "https://piroguetoolsuite.github.io/ppa/pirogue.list"
curl https://piroguetoolsuite.github.io/ppa/Key.gpg | sudo apt-key add -
sudo apt update
```