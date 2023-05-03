SQ-Mocu
====

sq1000000's fork of mocu

#### To install on Linux:

	wget -P /tmp  https://github.com/sq1000000/SQ-mocu/releases/download/1.0.0/SQ-Mocu.tar.xz
	tar -xf /tmp/SQ-Mocu.tar.xz -C /tmp
	mv /tmp/SQ-Mocu /home/$USER/.icons/
	flatpak --user override --filesystem=/home/$USER/.icons/:ro
	flatpak --user override --filesystem=/usr/share/icons/:ro
	

#### To install from source on Linux:

	git clone https://github.com/sq1000000/sq-mocu
	cd sq-mocu
	./make.sh
	cp dist/SQ-Mocu -r /home/$USER/.icons/
	cd ..
	rm -rf sq-mocu
	flatpak --user override --filesystem=/home/$USER/.icons/:ro
	flatpak --user override --filesystem=/usr/share/icons/:ro

Compilation Dependencies:

- Common bash, sed, grep, etc.
- rsvg-convert
- xmlstarlet
- xcursorgen
