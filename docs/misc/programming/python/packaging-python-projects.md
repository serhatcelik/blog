# Packaging Python Projects

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
