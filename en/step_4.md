<h2 class="c-project-heading--task">Print the letter at the new position.</h2>
--- task ---

Output the new character.

--- /task ---

Print the letter at the position in square brackets.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 11-12
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26
print(new_position)

new_character = alphabet[new_position]
print(new_character)
--- /code ---
</div>

<div class="c-project-output">
<pre>Please enter a character: e
7
h</pre>
</div>
