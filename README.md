# OrangePi_HomeAssistant
These commands will help you to install Home Assistant supervised on a Orange Pi Zero 2 or Orange Pi Zero 3
Note: it's recommanded to have at least 2GB of Ram.
You need to install Debian Kernel 6.1 (bookworm_server)
Available at http://www.orangepi.org/ 

## Install commands

```su```

```apt-get install sudo```

```sudo apt update && sudo apt upgrade -y && sudo apt autoremove -y```

```sudo -i```

```sudo reboot```

```apt --fix-broken install```

```apt-get install jq curl avahi-daemon apparmor-utils udisks2 libglib2.0-bin network-manager dbus wget -y```

```curl -fsSL get.docker.com | sh```

```wget https://github.com/home-assistant/os-agent/releases/download/1.6.0/os-agent_1.6.0_linux_aarch64.deb```

```dpkg -i os-agent_1.6.0_linux_aarch64.deb```

```wget https://github.com/home-assistant/supervised-installer/releases/latest/download/homeassistant-supervised.deb```

```sudo BYPASS_OS_CHECK=true dkpg -i homeassistant-supervised.deb```

```sudo apt-get install systemd-journal-remote```


```apt --fix-broken install```

## WIFI commands

```sudo apt-get install nmcli ```

```sudo nmcli dev ```

```sudo nmcli r wifi on```

```sudo nmcli dev wifi```

```sudo nmcli dev wifi connect 'your_wifi_name' password your_password```
