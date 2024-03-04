---
icon: material/help
---

# User Management

| Command | Description |
|:---|:---|
| `#!bash sudo` | Verilen komutu farklı bir kullanıcı olarak yürütür. |
| `#!bash su` | Belirtilen kullanıcı kimliğine geçer. |
| `#!bash useradd` | Yeni bir kullanıcı oluşturur. |
| `#!bash userdel` | Bir kullanıcı hesabını ve ilgili dosyaları siler. |
| `#!bash usermod` | Bir kullanıcı hesabını değiştirir. |
| `#!bash addgroup` | Sisteme bir grup ekler. |
| `#!bash delgroup` | Bir grubu sistemden kaldırır. |
| `#!bash passwd` | Kullanıcı parolasını değiştirir. |

## Questions

```text
Which option needs to be set to create a home directory for a new user using "useradd" command?
```

??? tip "Steps"

    ```bash
    man useradd | grep home
    ```

```text
Which option needs to be set to lock a user account using the "usermod" command? (long version of the option)
```

??? tip "Steps"

    ```bash
    man usermod | grep lock
    ```

```text
Which option needs to be set to execute a command as a different user using the "su" command? (long version of the option)
```

??? tip "Steps"

    ```bash
    man su | grep command
    ```
