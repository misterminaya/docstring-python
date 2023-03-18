## Docstring y Doctest

```python
def palindromo(sentence: str) -> bool:

    """ Permite conocer si un string es, o no, un palindromo.
    
    Args:
        sentence: string

    Returns:
        bool
    
    """

    sentence = sentence.lower().replace(' ','')
    return sentence == sentence[::-1]

```

### Instalar AutoDocstring Extenions 

Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.

```
ext install njpwerner.autodocstring
```

### Acceder a su documentación mediante la consola

```shell
palindromo.__doc__
```

```shell
help(palindromo)
```

### Ejecutar los Test DocString en la consola

```shell
python3 -m doctest main.py
```

```shell
python3 -m doctest main.py -v
```

### Realizando pruebas en un archivo externo

```shell
python3 -m doctest test_main.txt
```

```shell
python3 -m doctest test_main.txt -v
```


