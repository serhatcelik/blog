---
icon: material/help
search:
  boost: 0.5
---

# Working with Web Services

## Questions

```text
Find a way to start a simple HTTP server inside Pwnbox or your local VM using "npm". Submit the command that starts the web server on port 8080 (use the short argument to specify the port number).
```

??? tip "Steps"

    Gerekli yüklemeleri gerçekleştir:

    ```bash
    sudo apt update && sudo apt install -y npm && npm install http-server
    ```

    Yardım dosyasını görüntüle:

    ```bash
    http-server -h | grep port
    ```
