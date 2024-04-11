You can disable Fn Lock temporarily by using the command:

```bash
echo 0 | sudo tee /sys/module/hid_apple/parameters/fnmode
```

And permanently:

```bash
echo options hid_apple fnmode=0 | sudo tee -a /etc/modprobe.d/hid_apple.conf

sudo update-initramfs -u -k all
```