# VirtualBox Guest Additions

Gereklilikleri yükle (öncesinde tüm sistemi güncellemiş olmak tavsiye edilir):

```bash
sudo apt update && sudo apt install -y gcc build-essential dkms
```

Mount işlemini gerçekleştir:

```bash
sudo mount /dev/cdrom /mnt
```

Eklentiyi yükle:

```bash
sudo /mnt/VBoxLinuxAdditions.run
```
