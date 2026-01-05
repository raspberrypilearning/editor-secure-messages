<h2 class="c-project-heading--task">STEP TITLE</h2>
--- task ---
Print the new message on one line
--- /task ---

Store the new message in a variable, add each new character to it and print it at the end.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 4, 15, 16
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = input('Please enter the key: ')
key = int(key)
new_message = ''

message = input('Please enter a message: ')

for character in message:
	position = alphabet.find(character)

	new_position = (position + key) % 26

	new_character = alphabet[new_position]

	new_message += new_character
print(new_message)
--- /code ---
</div>

<div class="c-project-output">
<pre>Please enter the key: 5
Please enter a message: hello
mjqqt</pre>
</div>
