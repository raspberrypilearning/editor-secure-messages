<h2 class="c-project-heading--task">Wrap around</h2>
--- task ---

Use a `%` to force new position to 0 once it gets to 26.

--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 8
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26
print(new_position)
--- /code ---
</div>

<div class="c-project-output">
<pre>Please enter a character: y
1</pre>
</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

- Parentheses are needed around `position + key`

</div>
