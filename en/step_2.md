<h2 class="c-project-heading--task">Encrypt the character</h2>
--- task ---

Get the `position` of the character and add the `key` to it. 
Then store the result in a variable called `new_position`.

--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 6-9
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

<div class="c-project-callout c-project-callout--tip">
