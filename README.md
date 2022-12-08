## refind bootloader

그래픽 부트로더

### Build form soruce

* READ it first : [BUILDING.txt](./BUILDING.txt)

1) Download UDK2018 from
   https://github.com/tianocore/tianocore.github.io/wiki/UDK2018
   to /usr/local

2) cd /usr/local/[UDK2018 INSTALL PATH]
   `source edksetup.sh BaseTools`

3) Edit Conf/target.txt and change the following:
```
    - ACTIVE_PLATFORM = MdePkg/MdePkg.dsc
    - TARGET = RELEASE
    - TARGET_ARCH = X64
    - TOOL_CHAIN_TAG = GCC5
```

4) create debian package
   `dpkg-buildpackage`


### upstream 
* http://www.rodsbooks.com/refind/getting.html