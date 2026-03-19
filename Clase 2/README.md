# Programa en Python: Captura de Datos del Usuario

Este programa solicita al usuario información personal básica, validando cada entrada para asegurar que sea correcta.

---

## Funciones

### `pedir_texto(mensaje)`

Solicita al usuario un texto que contenga **solo letras**.

- Usa `input()` para recibir datos.
- Valida con `.isalpha()` que solo haya caracteres alfabéticos.
- Si la entrada es válida, la retorna.
- Si no, muestra un mensaje de error.

```python
def pedir_texto(mensaje):
    while True:
        dato = input(mensaje)
        if dato.isalpha():
            return dato
        else:
            print("Ingrese solo letras")