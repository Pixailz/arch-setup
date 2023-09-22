# arch-i3-setup

Script to install / setup arch with i3

## HOWTO

[Arch Install guide](https://wiki.archlinux.org/title/Installation_guide)

you should have at least internet connection in your booted live install of arch

because git isn't installed by default on live install, you can transfer the
repo with nc instead:

```bash
# on your actual PC
tar cvf - | nc <target_ip> 4444

# on the target PC
nc -lvp 4444 | tar xvf -
```
