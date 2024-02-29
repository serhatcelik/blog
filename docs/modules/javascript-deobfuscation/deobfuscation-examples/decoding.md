---
icon: material/help
search:
  boost: 2
---

# Decoding

## Base64

### Base64 Encode

```bash
echo https://www.hackthebox.eu/ | base64
```

```text title="Output"
aHR0cHM6Ly93d3cuaGFja3RoZWJveC5ldS8K
```

### Base64 Decode

```bash
echo aHR0cHM6Ly93d3cuaGFja3RoZWJveC5ldS8K | base64 -d
```

```text title="Output"
https://www.hackthebox.eu/
```

## Hex

### Hex Encode

```bash
echo https://www.hackthebox.eu/ | xxd -p
```

```text title="Output"
68747470733a2f2f7777772e6861636b746865626f782e65752f0a
```

### Hex Decode

```bash
echo 68747470733a2f2f7777772e6861636b746865626f782e65752f0a | xxd -p -r
```

```text title="Output"
https://www.hackthebox.eu/
```

## Caesar/Rot13

### Rot13 Encode

```bash
echo https://www.hackthebox.eu/ | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

```text title="Output"
uggcf://jjj.unpxgurobk.rh/
```

### Rot13 Decode

```bash
echo uggcf://jjj.unpxgurobk.rh/ | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

```text title="Output"
https://www.hackthebox.eu/
```

## Other Types of Encoding

[Cipher Identifier](https://www.boxentriq.com/code-breaking/cipher-identifier) gibi araçlar, kodlama türünü otomatik olarak belirlememize yardımcı olabilir.

## Questions

```text
Using what you learned in this section, determine the type of encoding used in the string you got at previous exercise, and decode it. To get the flag, you can send a 'POST' request to 'serial.php', and set the data as "serial=YOUR_DECODED_OUTPUT".
```

??? tip "Steps"

    Önceki bölümde elde edilen string değerini Cipher Identifier aracı ile analiz edersek, bu değerin Base64 ile kodlandığı bilgisini elde ederiz.

    Aşağıdaki komut ile Base64 kodlamasını tersine çevir:

    ```bash
    echo N2gxNV8xNV9hX3MzY3IzN19tMzU1NGcz | base64 -d
    ```

    ```text title="Output"
    7h15_15_a_s3cr37_m3554g3
    ```

    Ardından flag bilgisini elde etmek için aşağıda verilen cURL sorgusunu gerçekleştir:

    ```bash
    curl -X POST 94.237.55.163:45701/serial.php -d "serial=7h15_15_a_s3cr37_m3554g3"
    ```
