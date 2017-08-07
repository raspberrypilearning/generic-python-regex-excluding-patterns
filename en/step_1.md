- Sometimes you want to make substitutions but exclude certain characters when using **regex**.

- For instance you might want to replace all the characters that aren't vowels with underscores (`_`).

- By placing the character to ignore in square brackets and preceding them with the hat (`^`) character, the pattern becomes `[^aeiou]`.

	```python
	import re
	word = 'acetone'
	word = re.sub(r'[^aeiou]', '_', word)
	```
- This gives a result of `'a_e_o_e'`
