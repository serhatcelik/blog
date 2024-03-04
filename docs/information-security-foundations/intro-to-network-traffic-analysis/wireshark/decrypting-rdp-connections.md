---
icon: material/help
---

# Decrypting RDP connections

## Questions

```text
What user account was used to initiate the RDP connection?
```

??? tip "Steps"

    Wireshark `Edit` --> `Preferences` --> `Protocols` --> `TLS` yoluna ulaş.

    Burada `RSA keys list` --> `Edit` ile yeni bir pencere aç.

    Açılan pencerede `+` ile yeni bir anahtar ekle. Anahtara ait bilgiler aşağıda verildiği gibi olmalıdır:

    * IP address (10.129.43.29)
    * Port (3389)
    * Protocol (tpkt)
    * Key File (C:\Users\user\Documents\server.key)

    Anahtarı kaydet ve PCAP dosyasını yenile.

    Ardından aşağıdaki filtreyi gir:

    ```text
    rdp
    ```

    Çıkan sonuçlar incelendiğinde, `Remote Desktop Protocol` altında `userName` bilgisini bulabilirsin.
