# Constants

## const vs. #define

Aşağıdaki kod satırını ele alalım:

```c
#define MAX 9
```

Kaynak kodun herhangi bir yerinde `MAX` ifadesi görüldüğünde bu ifade `9` ifadesi ile değiştirilir (preprocessor tarafından).

Aşağıdaki kod satırını ele alalım:

```c
const int max = 9;
```

Buradaki `max` ifadesi sabit değişken olarak ele alınır ve bu değişken için hafızada gerekli yer tahsis edilir (compiler tarafından).

## Numeric Constants

| Decimal | Octal | Hexadecimal | Floating |
|:---|:---|:---|:---|
| 110 | 0156 | 0x6e | 110.000000 |

## Character Constants

| Single | String |
|:---|:---|
| 'n' | "n" |
