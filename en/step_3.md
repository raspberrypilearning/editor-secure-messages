<h2 class="c-project-heading--task">Encrypt the character</h2>

Add an encryption `key`.

Add the key to the original position and save the answer in a new variable called `new_position`.
Print the new position.

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

## Now run your code

Run your code, enter a character, and check that the new position number is printed.
