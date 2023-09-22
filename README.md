# arch-setup

Script to install / setup arch

## HOWTO

[Arch Install guide](https://wiki.archlinux.org/title/Installation_guide)

you only have to do [this](https://wiki.archlinux.org/title/Installation_guide#Connect_to_the_internet) part of the tutorial to be able to transfer the repo into the target host 

because git isn't installed by default on live install, you can do it with nc instead:

```bash
# on your actual PC
tar cvf - | nc <target_ip> 4444

# on the target PC
nc -lvp 4444 | tar xvf -
```
