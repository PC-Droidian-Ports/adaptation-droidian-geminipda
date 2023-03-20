# adaptation-droidian-geminipda
GeminiPDA adaptation 
This is the initial commit. 
Download the latest arm64 nightly image from droidian image repo at https://github.com/droidian-images/droidian/releases

To get droidian booting install TWRP onto your gemini. Allocate space to android and linux, boot into twrp, wipe data partition, from your computer and then run adb push droidian-OFFICIAL-phosh-phone-rootfs-api28-arm64-nightly_xxxxx.zip /tmp 
On the gemini select install
The navigate to /tmp

Select the droidian-OFFICIAL-phosh-phone-rootfs-api28-arm64-nightly_xxxxx.zip file. The zip file will install rootfs.img onto /data

reboot into linux and upload droidian-boot.img to the linux partition and run sudo dd if=droidian-boot.img of=/dev/disk/by-partlabel/boot2

reboot and boot the gemini using boot2 selection.

Currenty working:
Booting droidian
ssh using ssh droidian@10.15.19.82

To be done
Booting to gui
everything

