---
search:
  boost: 0.5
---

# Format Specifiers

| Format Specifier | Description | Supported Data Types |
|:---|:---|:---|
| `%c` | Character | `char`, `unsigned char` |
| `%d` | Signed integer | `short`, `unsigned short`, `int`, `long` |
| `%e` or `%E` | Scientific notation of float values | `float`, `double` |
| `%f` | Floating point | `float` |
| `%g` or `%G` | Similar as `%e` or `%E` | `float`, `double` |
| `%hi` | Signed integer (`short`) | `short` |
| `%hu` | Unsigned integer (`short`) | `unsigned short` |
| `%i` | Signed integer | `short`, `unsigned short`, `int`, `long` |
| `%l` or `%ld` or `%li` | Signed integer | `long` |
| `%lf` | Floating point | `double` |
| `%Lf` | Floating point | `long double` |
| `%lu` | Unsigned integer | `unsigned int`, `unsigned long` |
| `%lli` or `%lld` | Signed integer | `long long` |
| `%llu` | Unsigned integer | `unsigned long long` |
| `%o` | Octal representation of integer | `short`, `unsigned short`, `int`, `unsigned int`, `long` |
| `%p` | Address of pointer to `void*` | `void*` |
| `%s` | String | `char*` |
| `%u` | Unsigned integer | `unsigned int`, `unsigned long` |
| `%x` or `%X` | Hexadecimal representation of `unsigned` integer | `short`, `unsigned short`, `int`, `unsigned int`, `long` |
| `%n` | Prints nothing ||
| `%%` | Prints `%` character ||
