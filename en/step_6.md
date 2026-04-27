<h2 class="c-project-heading--task">Let the user enter their own key</h2>

Get the key from the user.

<h2 class="c-project-heading--explainer">Follow these instructions</h2>

Remove the unecessary print statement.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2, 3, 10, 12
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = input('Please enter the key: ')
key = int(key)

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26

new_character = alphabet[new_position]
print('The new character is: ', new_character)
--- /code ---
</div>

<div class="c-project-output">
<pre>Please enter the key: 5
Please enter a character: f
The new character is:  k</pre>
</div>

### Debugging

<div class="c-project-callout c-project-callout--debug">

- Make sure you have used `int` to convert the input key to an integer (number).

</div>

## Now run your code

Run your code, enter a key and a character, and check that the new encrypted character matches your key.
