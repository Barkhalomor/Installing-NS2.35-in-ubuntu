# Installing-NS2.35-in-ubuntu
Installation of NS2.35 in ubuntu step wise prodedure

1.	sudo bash
2.	sudo apt-get update
3.	Extract : ns tar file
4.	cd/home/autoroot
5.	tar -xvzf ns-allinone-2.35.tar.gz
6.	sudo apt-get install gcc-4.4 	//since compiler is already installed.
7.	cd /home/autoroot/ns-allinone-2.35/ns-2.35/linkstate
8.	gedit ls.h 	//replace the erase(image 1) with this—>erase (image 2) and save the file.
9.	cd /home/autoroot/ns-allinone-2.35
10.	sudo ./install
11.	gedit .bashrc
12.	Start gedit and open /root/.bashrc file. Add the following 5 lines at the end of the file.

export PATH=$PATH:/root/ns2/ns-allinone-2.35/bin:/root/ns2/ns-allinone-2.35/tcl8.5.10/unix/:/root/ns2/ns-allinone-2.35/tk8.5.10/unix/
	
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/root/ns2/ns-allinone-2.35/otcl-1.14/:/root/ns2/ns-allinone-2.35/lib

export TCL_LIBRARY=/root/ns2/ns-allinone-2.35/tcl8.5.10/library/:/root/ns2/ns-allinone-2.35/tk8.5.10/library/

export NS=/root/ns2/ns-allinone-2.35/ns-2.35
export NSVER=2.35
13.	Then logoff from root user and relogin and execute type ns at the terminal for checking.

