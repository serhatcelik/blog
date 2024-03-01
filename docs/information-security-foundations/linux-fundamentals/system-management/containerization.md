---
icon: material/circle-small
search:
  boost: 0.5
---

# Containerization

## Install LXC

```bash
sudo apt-get install -y lxc lxc-utils
```

## Securing LXC

LXC (Linux Containers) için kullanılan kaynaklar sınırlanarak güvenlik artırılabilir.

Kapsayıcının kullanabileceği işlemci süresini ayarla:

```bash
echo "lxc.cgroup.cpu.shares = 512" >> /usr/share/lxc/config/lxc.conf
```

Kapsayıcının kullanabileceği maksimum bellek miktarını ayarla:

```bash
echo "lxc.cgroup.memory.limit_in_bytes = 512M" >> /usr/share/lxc/config/lxc.conf
```
