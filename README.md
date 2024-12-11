# NS3_Project
install ns3 on ubuntu

$ sudo apt update
$ sudo apt install g++ python3 cmake ninja-build git gir1.2-goocanvas-2.0 python3-gi python3-gi-cairo python3-pygraphviz gir1.2-gtk-3.0 ipython3 tcpdump wireshark sqlite sqlite3 libsqlite3-dev qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools openmpi-bin openmpi-common openmpi-doc libopenmpi-dev doxygen graphviz imagemagick python3-sphinx dia imagemagick texlive dvipng latexmk texlive-extra-utils texlive-latex-extra texlive-font-utils libeigen3-dev gsl-bin libgsl-dev libgslcblas0 libxml2 libxml2-dev libgtk-3-dev lxc-utils lxc-templates vtun uml-utilities ebtables bridge-utils libxml2 libxml2-dev libboost-all-dev 

$ mkdir workspace
$ cd workspace
$ wget https://www.nsnam.org/releases/ns-allinone-3.40.tar.bz2
$ tar xvf ns-allinone-3.40.tar.bz2
$ cd ns-allinone-3.40/ns-3.40/
$ ./ns3 clean
$ ./ns3 configure --build-profile=debug --enable-examples --enable-tests --disable-python --disable-werror
$ ./ns3 build

