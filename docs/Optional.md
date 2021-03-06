# Optional

- `v::optional(v $rule)`

Validates if the given input is optional or not. By _optional_ we consider `null`
or an empty string (`''`).

```php
v::optional(v::alpha())->validate(''); // true
v::optional(v::digit())->validate(null); // true
```


***
See also:

  * [NoWhitespace](NoWhitespace.md)
  * [NotBlank](NotBlank.md)
  * [NotEmpty](NotEmpty.md)
  * [NotOptional](NotOptional.md)
  * [NullType](NullType.md)
