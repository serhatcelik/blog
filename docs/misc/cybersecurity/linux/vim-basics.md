# Vim Basics

## Install Vim

Vim yazılımını yüklemek için aşağıdaki komut kullanılabilir:

```bash
sudo pacman -Syy vim
```

## 1. Normal Mode

!!! info "Vim Motions"

    Vim motions (hareketler), imleci hareket ettirmek için kullanılan tuşlardır.

| Motion | Description |
|:---|:---|
| ++lower-j++ | Satır boyu aşağı (++down++) ilerle. |
| ++lower-k++ | Satır boyu yukarı (++up++) ilerle. |
| ++lower-h++ | Karakter boyu sola (++left++) ilerle. |
| ++lower-l++ | Karakter boyu sağa (++right++) ilerle. |
| ++lower-w++ | Kelime boyu sağa ilerle. |
| ++lower-b++ | Kelime boyu sola ilerle. |

!!! info "Count + Motion"

    Motion tuşları sayılar ile birlikte kullanılabilir. Örneğin ++3++ ++lower-k++ tuş kombinasyonu ile mevcut satırdan 3 satır yukarıda bulunan satıra hareket edilebilir.

| Command | Description |
|:---|:---|
| ++lower-d++ ++lower-d++ | Mevcut satırı sil. |
| ++lower-u++ | Geri al. |
| ++control+lower-r++ | Yinele. |
