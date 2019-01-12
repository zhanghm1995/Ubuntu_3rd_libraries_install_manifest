### Usages
This repository is for backuping the install_manifest.txt files of some 3rd libraries that are installed from source, especially those libraries installed by below command: 
```
$ sudo make install
```
This command will generate `intall_manifest.txt` file in **build** folder and can be used to uninstall those libraries intalled files (headers、libraries and so on) in your system path.

Details about how to use intall_manifest.txt to uninstall libraries can refer to: 
https://cmake.org/Wiki/CMake_FAQ#Can_I_do_.22make_uninstall.22_with_CMake.3F

**uninstall command**:
```
xargs rm < install_manifest.txt
```
