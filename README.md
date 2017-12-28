# WiSystem

## Get repositories

    cd $HOME

    mkdir test

    cd test

    git clone --progress https://github.com/WiSystem/buildroot_ext.git

    wget https://buildroot.org/downloads/buildroot-2017.02.tar.gz

    tar xf buildroot-2017.02.tar.gz

    cd buildroot-2017.02

    make BR2_EXTERNAL=../buildroot_ext list-defconfigs

# Select defconfig

    make grinn_liteboard_defconfig
    make uavx_35i00_defconfig
    make uavx_37i00_defconfig
    
    make all

## How to use Qt

    cd $HOME

    export PATH=$HOME/test/buildroot-2017.02/output/host/usr/bin:${PATH}

    mkdir qt

    cd qt

    git clone --progress https://github.com/WiSystem/QtVersion.git

    cd QtVersion

    qmake 

    make


