The image was build with the LTS version - 2019.02.4 - of [BuildRoot](https://buildroot.org/downloads/buildroot-2019.02.4.tar.gz).

1. Download & Extract BuildRoot
2. Copy the content of the repository-buildroot folder into the folders of downloaded buildroot version
    1. `cp -r repository/buildroot/boards/* download/buildroot/boards/`
    2. `cp -r repository/buildroot/configs/* download/buildroot/configs/`
    3. `cp -r repository/buildroot/package/* download/buildroot/package/`
4. Add the content of the file buildroot/packages/Config.in.additions add the end of file packages/Config.in
5. sudo apt install libncurses5-dev
6. make simplyRetro-z5_defconfig
7. make menuconfig
8. make
