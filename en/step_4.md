## Variable keys

--- task ---

Modify your program, so that the user can enter their own key to use. 

You'll need to get the user's input, and store it in the `key` variable.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2-3
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

--- /task ---
