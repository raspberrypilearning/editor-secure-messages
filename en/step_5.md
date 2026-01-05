## Encrypting entire messages

Instead of just encrypting and decrypting messages one character at a time, let's change the program to encrypt entire messages!

--- task ---

Change your code to store the user's message and not just one character.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = input('Please enter the key: ')
key = int(key)

message = input('Please enter a message: ')

position = alphabet.find(character)

new_position = (position + key) % 26

new_character = alphabet[new_position]
print('The new character is: ', new_character)
--- /code ---

--- /task ---

--- task ---

Add a `for` loop to your code, and indent the rest of the code so that it is repeated for each character in the message.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 7
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = input('Please enter the key: ')
key = int(key)

message = input('Please enter a message: ')

for character in message:
	position = alphabet.find(character)

	new_position = (position + key) % 26

	new_character = alphabet[new_position]
	print('The new character is: ', new_character)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

Test your code. 

You should see that each character in the message is encrypted and printed one at a time.

```
Please enter a message: hello
The new character is:  k
The new character is:  h
The new character is:  o
The new character is:  o
The new character is:  r
```

--- /task ---

--- task ---

Create a variable to store the new encrypted message.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 4
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
	print('The new character is: ', new_character)
--- /code ---

--- /task ---

--- task ---

Add each encrypted character to your `new_message` variable.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 15-16
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
	print('The new character is: ', new_character)
	new_message += new_character
	print(new_message)
--- /code ---

--- /task ---

--- task ---

Delete the indentation before the `print` statement so the encrypted message will only be displayed once at the end. 

You can also delete the other print statement that prints the characters.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 14, 16
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

--- /task ---
