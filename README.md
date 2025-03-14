## Operadores de Comparación en PHP

Los operadores de comparación en PHP permiten comparar valores y determinar su relación.

### 📌 Lista de Operadores de Comparación

| Operador    | Descripción                            | Devuelve `true` si...                                                                                                      |
| ----------- | -------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `$a == $b`  | **Igual**                              | `$a` es igual a `$b` después de la conversión de tipos.                                                                    |
| `$a === $b` | **Idéntico**                           | `$a` es igual a `$b`, y son del mismo tipo.                                                                                |
| `$a != $b`  | **No igual**                           | `$a` no es igual a `$b` después de la conversión de tipos.                                                                 |
| `$a <> $b`  | **No igual**                           | `$a` no es igual a `$b` después de la conversión de tipos.                                                                 |
| `$a !== $b` | **No idéntico**                        | `$a` no es igual a `$b`, o no son del mismo tipo.                                                                          |
| `$a < $b`   | **Menor que**                          | `$a` es estrictamente menor que `$b`.                                                                                      |
| `$a > $b`   | **Mayor que**                          | `$a` es estrictamente mayor que `$b`.                                                                                      |
| `$a <= $b`  | **Menor o igual a**                    | `$a` es menor o igual a `$b`.                                                                                              |
| `$a >= $b`  | **Mayor o igual a**                    | `$a` es mayor o igual a `$b`.                                                                                              |
| `$a <=> $b` | **Operador combinado (nave espacial)** | Retorna un `int` menor que, igual a, o mayor que `0` cuando `$a` es menor que, igual a, o mayor que `$b`, respectivamente. |

### 📌 Ejemplo de Uso

```php
$a = 5;
$b = "5";

var_dump($a == $b);  // true (comparación después de conversión de tipos)
var_dump($a === $b); // false (no son del mismo tipo)
var_dump($a <=> $b); // 0 (son iguales)
