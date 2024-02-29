---
icon: material/help
search:
  boost: 0.5
---

# Navigation

| Command | Description |
|:---|:---|
| `#!bash ls` | Dizin içeriğini listeler. |
| `#!bash ls -a` | Dizin içeriğini gizli dosyalarla birlikte listeler. |
| `#!bash ls -l` | Dizin içeriğini daha fazla bilgi gösterecek şekilde listeler. |
| `#!bash cd` | Dizinler arasında gezinmeyi sağlar. |
| `#!bash cd ~` | Mevcut kullanıcının ev dizinine geçiş yapar. |
| `#!bash cd -` | Son bulunulan dizine geri döner. |
| `#!bash cd ..` | Bir üst dizine geçiş yapar. |
| `#!bash clear` | Shell ekranını temizler. |
| `#!bash clear -x` | Shell ekranını kısmen temizler. |

## Questions

```text
What is the name of the hidden "history" file in the htb-user's home directory?
```

??? tip "Steps"

    ```bash
    cd ~ && ls -a
    ```

```text
What is the index number of the "sudoers" file in the "/etc" directory?
```

??? tip "Steps"

    ```bash
    ls -i /etc/sudoers
    ```
