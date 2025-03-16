Environment:
    Ubuntu 14.04.6 server 64bit
    https://releases.ubuntu.com/14.04/ubuntu-14.04.6-server-amd64.iso

Procedure:
    sudo apt-get update
    sudo apt-get -y install bison flex gettext patch texinfo lzma build-essential zip gcc-multilib
    sudo mkdir /usr/local/ARC
    chmod a+x QEnvInstaller-v1.2.bin
    sudo ./QEnvInstaller-v1.2.bin
    sudo mv /usr/local/ARC/arcp1 /usr/local/ARC/arcp1_v1.2
    tar -jxvf TEFDEF_r3595.tar.bz2
    cd TEFDEF_r3595/
    ./build_tef.sh
    
Result:
    After building code complete, the FW file will be in images/ folder. The FW filename is "GL_g8.7_RG3110W0.6.8gpl.img". 
