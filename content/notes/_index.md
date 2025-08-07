

- recently working on an Ubuntu virtual machine, trying to enable copying and pasting between the host and guest, was not playing well with Wayland
	- Thank you Doron: https://itsfoss.community/t/switching-from-wayland-to-x11-in-ubuntu-22-04/10723
	- `sudo vim /etc/gdm3/custom.conf`
	- Uncomment `#WaylandEnable=false`
	- `systemctl restart gdm3`
- check if you are running X11 or Wayland
	- `loginctl`, find your session
	- `loginctl show-session (#) -p Type`

- manually installing packages on Ubuntu
	- `sudo dpkg -i (deb file)`
