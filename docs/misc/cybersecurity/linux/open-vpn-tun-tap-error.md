# OpenVPN TUN/TAP Error

Sorunu çözmek için character tipinde (`c`) bir cihaz oluşturmak gerekebilir. Bu tipteki cihazlar, fiziksel olarak adreslenebilir depolama ortamlarına sahip değillerdir. Diğer cihazlarla iletişim kurmak için tekil karakterler (bytes, octets) gönderir ve alırlar:

```bash
sudo mknod /dev/net/tun c 10 200
```

| Command | Description |
|:---|:---|
| `/dev/net/tun` | Oluşturulacak dosyanın ismi. |
| `c` | Oluşturulacak dosyanın tipi. |
| `10` | Oluşturulacak dosyanın major numarası. |
| `200` | Oluşturulacak dosyanın minor numarası. |

Oluşturulan dosyanın niteliklerini kontrol edelim:

| File type | Owner | Group | Others | Number of hard links | User | Group | Major number | Minor number | Date | File name |
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
| `c` | `rw-` | `rw-` | `rw-` | `1` | `root` | `root` | `10` | `200` | `Mar 11 10:50` | `/dev/net/tun` |

Major ve minor numaralarını incelemek için [bu](https://www.kernel.org/doc/Documentation/admin-guide/devices.txt) site kullanılabilir. Bu örnek için bakacak olursak:

| Major number (10) | Minor number (200) |
|:---|:---|
| Non-serial mice, misc features | TAP/TUN network device |