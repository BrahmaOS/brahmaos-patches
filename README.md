# brahmaos-patches
Include all brahmaos patches based AOSP.

BrahmaOS source code base is Android Oreo, tag android-8.1.0_r22

Step1: [Download AOSP code](https://source.android.com/setup/build/downloading)

```shell
$ repo init -u https://android.googlesource.com/platform/manifest -b android-8.1.0_r22
$ repo sync
```

Step2: Download brahmaos-patches

```shell
$ cd <AOSPDIR>
$ git clone https://github.com/BrahmaOS/brahmaos-patches
$ ./brahmaos-patches/install.sh
```



