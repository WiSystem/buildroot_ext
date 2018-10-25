# WiSystem

## Get repositories

    cd $HOME

    mkdir test

    cd test

    git clone --progress https://github.com/WiSystem/buildroot_ext.git

    wget https://buildroot.org/downloads/buildroot-2018.08.2.tar.gz

    tar xf buildroot-2018.08.2.tar.gz

    cd buildroot-2018.08.2

    make BR2_EXTERNAL=../buildroot_ext list-defconfigs

# Select defconfig

    make grinn_liteboard_defconfig
    
    make uavx_35i00_defconfig
    make uavx_37i00_defconfig
    
# Build

    make all

## How to use Qt

    cd $HOME

    export PATH=$HOME/test/buildroot-2018.08.2/output/host/usr/bin:${PATH}

    mkdir qt

    cd qt

    git clone --progress https://github.com/WiSystem/QtVersion.git

    cd QtVersion

    qmake 

    make


