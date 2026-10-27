qemu-raspi3-playground
======================
```
#!/bin/sh
qemu-system-aarch64 \
  -machine raspi3b \
  -smp 4,cores=1 \
  -kernel buildroot/output/images/u-boot.bin \
  -serial null \
  -serial mon:stdio \
  -nographic \
  -drive file=buildroot/output/images/2022-01-28-raspios-bullseye-arm64-lite.img,format=raw,if=sd
```
### Tutorials
- [ECEN5713](https://sites.google.com/colorado.edu/ecen5713/home)
  - [lnxblog/ecen_5713_final_project](https://github.com/lnxblog/ecen_5713_final_project/tree/main)
