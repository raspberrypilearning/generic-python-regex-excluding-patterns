- Soms wil je bij het gebruikmaken van regex vervangingen terwijl je bepaalde tekens uitsluit. Je wilt bijvoorbeeld alle tekens in je tekenreeks die geen klinkers zijn, vervangen door onderstrepingstekens (`_`).

- Je kunt dit doen door de te negeren tekens tussen vierkante haken te plaatsen en ze te laten voorafgaan door het hoed (`^`) -teken, zodat het patroon `[^aeiou]` wordt.

    ```python
    import re
woord = 'aceton'
woord = re.sub(r'[^aeiou]', '_', woord)
    ```
- Dit geeft je als resultaat `'a_e_o_e'`.
