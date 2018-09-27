# brahmaos-patches
Include all BrahmaOS patches based AOSP.

BrahmaOS source code base is Android Oreo, tag android-8.1.0_r22

**Step1: [Download AOSP code](https://source.android.com/setup/build/downloading)**

```shell
$ repo init -u https://android.googlesource.com/platform/manifest -b android-8.1.0_r22
$ repo sync
```

**Step2: Download brahmaos-patches**

```shell
$ cd <AOSPDIR>
$ git clone https://github.com/BrahmaOS/brahmaos-patches
$ ./brahmaos-patches/install.sh
```
**Step3: Compile BrahmaOS**

```shell
$ cd <AOSPDIR>
$ source build/envsetup.sh
$ lunch aosp_angler-userdebug
$ make -j16
```

**Step4: Flash the image**

First you should connect the USB cable with the device,  
then press power + Volume down button for more than 10 seconds  
to enter fastboot mode.

``` shell
$ sudo fastboot flash vendor out/target/product/angler/vendor.img
$ sudo fastboot flash system out/target/product/angler/system.img
```


