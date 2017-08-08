- Sometimes when using regex, you might want to make substitutions while excluding certain characters. For instance, you might want to replace all the characters in your string that aren't vowels with underscores (`_`).

- You can do this by placing the characters to ignore in square brackets and preceding them with the hat (`^`) character, so the pattern becomes `[^aeiou]`.

	```python
	import re
	word = 'acetone'
	word = re.sub(r'[^aeiou]', '_', word)
	```
- This will give you the result `'a_e_o_e'`.
