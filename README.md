# waveshare35-rpi3b-ubuntu-20.04-64

This Ansible playbook will configure your Raspberry Pi Model 3 running Ubuntu Server 20.04 (64-bit) to work with a Waveshare 3.5inch RPi LCD (A).

![](http://www.lcdwiki.com/images/4/44/MPI3501-001.jpg)

[Product Page](https://www.waveshare.com/product/3.5inch-RPi-LCD-A.htm)

Other links:
+ [Waveshare Wiki](https://www.waveshare.com/wiki/3.5inch_RPi_LCD_(A))
+ [Official GitHub](https://github.com/waveshare/LCD-show)
+ [LCD Wiki](http://www.lcdwiki.com/3.5inch_RPi_Display)
+ [GitHub: lcdwiki/LCD-show-ubuntu](https://github.com/lcdwiki/LCD-show-ubuntu)

Instructions
---

_**Note:** Execute all steps as root_


a. Install ansible

```
# apt install ansible
```

b. Download the ansible repo to '/root'

```none
# cd

# git clone "https://github.com/victorbrca/waveshare35-rpi3b-ubuntu-20.04-64.git"
```

c. Change into the project directory and run the Ansible playbook

```
# cd waveshare35-rpi3b-ubuntu-20.04-64

# ansible-playbook playbook.yaml
```

_**Note:** The update/upgrade part of the install takes quite a while_

```none
# ansible-playbook playbook.yaml
[WARNING]: provided hosts list is empty, only localhost is available. Note that the implicit localhost
does not match 'all'

PLAY [localhost] ****************************************************************************************

TASK [Gathering Facts] **********************************************************************************
ok: [localhost]

TASK [packages : Running apt-get update and upgrade] ****************************************************
```

- - -

**Reference:**
+ [GitHub: goodft/LCD-show](https://github.com/goodtft/LCD-show)
+ [Raspberry Pi Forums: 480x320 Touchscreen](https://www.raspberrypi.org/forums/viewtopic.php?p=977889#p977889)
+ [Ubuntu Mate Community: LCD 3.5 XPT2046 Touch screen does not work on Raspberry Pi 3 Model B+](https://ubuntu-mate.community/t/lcd-3-5-xpt2046-touch-screen-does-not-work-on-raspberry-pi-3-model-b/19261/3)
+ [GitHub: notro/fbtft](https://github.com/notro/fbtft/issues/433)
+ [GitHub:  swkim01/waveshare-dtoverlays](https://github.com/swkim01/waveshare-dtoverlays)
