<h2 class="c-project-heading--task">Encrypt the character</h2>
--- task ---

Add an encryption `key`.
Add it to the position.
Print the new position.

--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2, 8, 9
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = position + key
print(new_position)
--- /code ---
</div>

<div class="c-project-output">
<pre>Please enter a character: e
7</pre>
</div>

