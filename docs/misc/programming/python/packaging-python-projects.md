---
search:
  boost: 0.5
---

# Packaging Python Projects

## Python 3.x for Linux

Gereklilikleri yükle:

```bash
sudo apt update && sudo apt install software-properties-common && sudo add-apt-repository ppa:deadsnakes/ppa
```

Gerekli Python sürümünü yükle:

```bash
sudo apt update && sudo apt install python3.11
```

PIP dosyasını edin ve yükle:

```bash
curl -sS https://bootstrap.pypa.io/get-pip.py | python3.11
```

PIP sürümünü güncelle:

```bash
python3.11 -m pip install -U pip
```

## Test PyPI

Gereklilikleri yükle ve geçerli dizindeki dosyaları derle:

```bash
python -m pip install -U twine build && python -m build
```

Dosyaları karşıya (Test PyPI) yükle (kullanıcı adı olarak `__token__` ve parola olarak Token değerini ver):

```bash
python -m twine upload -r testpypi dist/*
```

PIP ile istenen kurulumu gerçekleştir:

```bash
python -m pip install -i https://test.pypi.org/simple/ avsub
```

## PyPI

Gereklilikleri yükle ve geçerli dizindeki dosyaları derle:

```bash
python -m pip install -U twine build && python -m build
```

Dosyaları karşıya (PyPI) yükle (kullanıcı adı olarak `__token__` ve parola olarak Token değerini ver):

```bash
python -m twine upload dist/*
```

PIP ile istenen kurulumu gerçekleştir:

```bash
python -m pip install avsub
```
