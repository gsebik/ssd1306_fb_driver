# ssd1306_fb_driver


## Install driver

```bash
make

sudo insmod ssd1306fb.ko

echo dtoverlay=ssd1306fb | sudo tee -a /boot/firmware/config.txt

dtc -@ -I dts -O dtb -o ssd1306fb.dtbo ssd1306fb-overlay.dts

sudo cp ssd1306fb.dtbo /boot/overlays/

```

