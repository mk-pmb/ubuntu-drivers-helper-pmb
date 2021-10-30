
```text
# ubuntu-drivers devices
== /sys/devices/pci0000:00/0000:00:01.0/0000:05:00.0 ==
modalias : pci:v000010DEd00000622sv00001043sd000082FCbc03sc00i00
vendor   : NVIDIA Corporation
model    : G94 [GeForce 9600 GT]
driver   : nvidia-340 - distro non-free recommended
driver   : xserver-xorg-video-nouveau - distro free builtin

# ubuntu-drivers list
nvidia-340

# lspci -ks 05:00.0
05:00.0 VGA compatible controller: NVIDIA Corporation G94 [GeForce 9600 GT] (rev a1)
        Subsystem: ASUSTeK Computer Inc. G94 [GeForce 9600 GT]
        Kernel driver in use: nouveau
        Kernel modules: nvidiafb, nouveau
```

* `nouveau` works
* `nvidia-340` makes X fail to start with error
  `(EE) Fatal server error:(EE) no screens found(EE)`



