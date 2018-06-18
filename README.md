# ma-c-tools

## How to prepare source files for c-tools package

1. ソースファイルの準備 (ホスト上で)

        VERSION=0.6.2
        VERSION_TGZ=062
        cd $HOME/vagrant/data/src
        rm -rf C-TOOLS$VERSION_TGZ c-tools_$VERSION
        wget -O C-TOOLS$VERSION_TGZ.tgz https://sourceforge.net/projects/c-tools/files/C-TOOLS$VERSION_TGZ.tgz/download
        tar zxvf C-TOOLS$VERSION_TGZ.tgz
        mv -f C-TOOLS$VERSION_TGZ c-tools_$VERSION
        tar zcvf c-tools_$VERSION.orig.tar.gz c-tools_$VERSION
        rm -rf C-TOOLS$VERSION_TGZ.tgz c-tools_$VERSION
