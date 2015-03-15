Install qimsys from source

# Download #

Download qimsys-x.y.z.tar.gz from [Download page](http://code.google.com/p/qimsys/downloads/list)
```
$ tar zxvf qimsys-x.y.z.tar.gz
```
Or

Get latest one from repository
```
$ git clone git://gitorious.org/qimsys/qimsys.git qimsys
```

# Configuration #

```
$ mkdir build
$ cd build
$ qmake ../qimsys(-x.y.z)/qimsys.pro
```

## Options ##
  * PREFIX=/usr
  * QT\_IM\_MODULE\_DIR=/usr/lib/qt4/plugins/inputmethods
  * GTK\_IM\_MODULE\_DIR=/usr/lib/gtk-2.0/2.10.0/immodules

# Build #
```
$ make
```

# Install #
```
$ make -n install
$ sudo make install
```

# Change IM settings #
add below to ~/.profile, ~/.xprofile or so
```
export XMODIFIERS=@im=qimsys
export QT_IM_MODULE=qimsys
export GTK_IM_MODULE=qimsys
```

You may need reboot or relogin after the setup.