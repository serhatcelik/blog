---
icon: material/help
search:
  boost: 2
---

# System Information

| Command | Description |
|:---|:---|
| `#!bash whoami` | Geçerli kullanıcı adını görüntüler. |
| `#!bash id` | Kullanıcı kimliğini görüntüler. |
| `#!bash hostname` | Mevcut makinenin adını ayarlar veya görüntüler. |
| `#!bash uname` | Sistem donanımı hakkındaki bilgileri görüntüler. |
| `#!bash pwd` | Çalışma dizini adını görüntüler. |
| `#!bash ifconfig` | Ağ arayüzü parametrelerini yapılandırmak için kullanılır. |
| `#!bash netstat` | Ağ durumunu görüntüler. |
| `#!bash ss` | Soketleri araştırmak için kullanılır. |
| `#!bash ps` | İşlem durumunu görüntüler. |
| `#!bash who` | Kimin oturum açtığını görüntüler. |
| `#!bash env` | Mevcut ortamı görüntüler. |
| `#!bash lsblk` | Blok cihazlarını listeler. |
| `#!bash lsusb` | USB cihazlarını listeler. |
| `#!bash lsof` | Açılan dosyaları listeler. |
| `#!bash lspci` | PCI cihazlarını listeler. |

## Questions

```text
Find out the machine hardware name and submit it as the answer.
```

??? tip "Steps"

    Öncelikle makineye SSH ile bağlanmalıyız:

    ```bash
    ssh htb-student@10.129.200.91
    ```

    Ardından aşağıdaki komutu girerek cevabı alabiliriz:

    ```bash
    uname -m
    ```

```text
What is the path to htb-student's home directory?
```

??? tip "Steps"

    ```bash
    cd ~ && pwd
    ```

```text
What is the path to the htb-student's mail?
```

??? tip "Steps"

    ```bash
    env | grep mail
    ```

```text
Which shell is specified for the htb-student user?
```

??? tip "Steps"

    Açık olan dosyalardan mevcut işlemin PID bilgisine göre listele:

    ```bash
    lsof -p $$
    ```

```text
Which kernel version is installed on the system? (Format: 1.22.3)
```

??? tip "Steps"

    ```bash
    uname -r
    ```

```text
What is the name of the network interface that MTU is set to 1500?
```

??? tip "Steps"

    ```bash
    ifconfig | grep "mtu 1500"
    ```
