# PiRogue Debian packages

## Install Raspberry Pi OS
To install Raspberry Pi OS, please follow [the official documentation](https://www.raspberrypi.com/documentation/computers/getting-started.html#installing-the-operating-system). You will have to install **Raspberry Pi OS Lite**.

Once installed, you have to [enable SSH](https://www.raspberrypi.com/documentation/computers/remote-access.html#ssh).

If you plan to use the PiRogue in a production environment (office, lab), we suggest you follow the [securing your Raspberry Pi guide](https://www.raspberrypi.com/documentation/computers/configuration.html#securing-your-raspberry-pi).


## Install the PiRogue packages repository

To install PiRogue packages repository on you fresh Debian installation, execute the following command in a terminal:

```bash
sudo curl -o /etc/apt/sources.list.d/pirogue.list https://pts-project.org/ppa/pirogue.list
sudo curl -o /etc/apt/trusted.gpg.d/pirogue.asc   https://pts-project.org/ppa/Key.gpg
sudo apt update
```

## Installation on Raspberry Pi 
For the moment, we only support Raspberry Pi having at least 1GB of RAM:
* Raspberry Pi 3 Model B
* Raspberry Pi 3 Model B+
* Raspberry Pi 4 Model B - 1GB
* Raspberry Pi 4 Model B - 2GB
* Raspberry Pi 4 Model B - 4GB
* Raspberry Pi 4 Model B - 8GB

To install PiRogue features, run the following command
```bash
sudo apt install pirogue-base
```

During the installation, when prompted, you will have to answer:
* `Yes` to save iptables rules for IP v4
* `Yes` to save iptables rules for IP v6
* `Yes` to allow non-root users to capture network traffic 

![Allow non-root users to capture network traffic ](/img/install-1.png)



**Important note** Suricata is disabled on devices having less then 1.5GB of RAM.

## Installation on a regular PC
For more details, check [the corresponding documentation](https://pts-project.org/docs/recipes/turn-a-regular-pc-into-a-pirogue/).

To install PiRogue features, run the following command
```bash
sudo apt install pirogue-base-pc
```