- A veces, al usar expresiones regulares, es posible que desees realizar sustituciones mientras excluyes ciertos caracteres. Por ejemplo, puede que quieras reemplazar todos los caracteres de tu cadena que no sean vocales con guiones bajos (`_`).

- Puedes hacer esto colocando los caracteres para ignorar entre corchetes cuadrados y precediéndolos con el carácter del sombrero (`^`), así que el patrón se convierte en `[^aeiou]`.

    ```python
    import re
    palabra = 'acetona'
    palabra = re.sub(r'[^aeiou]', '_', palabra)
    ```
- Esto te dará el resultado `'a_e_o_a'`.
