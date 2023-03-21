# PiRogue Debian packages

## Install the PiRogue packages repository

To install PiRogue packages repository on you fresh Debian installation, execute the following command in a terminal:

```bash
sudo curl -o /etc/apt/sources.list.d/pirogue.list https://pts-project.org/ppa/pirogue.list
sudo curl -o /etc/apt/trusted.gpg.d/pirogue.asc   https://pts-project.org/ppa/Key.gpg
sudo apt update
```

To install PiRogue features, run the following command
```bash
sudo apt install pirogue-base-pc
```

## Installation on Raspberry Pi 
Check the corresponding [documentation on PTS's website](https://pts-project.org/docs/pirogue/build-a-pirogue/).

## Installation on a regular PC
Check the corresponding [documentation on PTS's website](https://pts-project.org/docs/recipes/turn-a-regular-pc-into-a-pirogue/).
