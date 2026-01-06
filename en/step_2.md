<h2 class="c-project-heading--task">Encrypt the character</h2>
--- task ---

Print the `position` of the character. 

--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5-7
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'

character = input('Please enter a character: ')

position = alphabet.find(character)

print(position)
--- /code ---
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

- The letter `a` is at position `0` in the alphabet.

</div>

<div class="c-project-output">
<pre>Please enter a character: e
5</pre>
</div>

<div class="c-project-callout c-project-callout--tip">
