## Encrypting letters

Write a Python program to encrypt a single character.

--- task ---

Open the [Secure Messages starter project](https://editor.raspberrypi.org/en/projects/secure-messages-starter){:target="_blank"}.

--- /task ---

--- task ---

Instead of drawing the alphabet in a circle, write it out as an `alphabet` variable.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 1
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
--- /code ---

--- /task ---

Each letter of the alphabet has a position, starting at position 0. So the letter 'a' is at position 0 of the alphabet, and 'c' is at position 2.

--- task ---

Output a letter from your `alphabet` variable by printing the letter at the position in square brackets.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2-4
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
print(alphabet[0])
print(alphabet[6])
print(alphabet[19])
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

You can delete the `print` statements once you've tried this out.

--- /task ---

--- task ---

Store the `key` in a variable.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3
--- /code ---

--- /task ---

--- task ---

Ask the user for a single letter (called a `character`) to encrypt.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 4
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')
--- /code ---

--- /task ---

--- task ---

Find the `position` of the `character`.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 6
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)
--- /code ---

--- /task ---

--- task ---

You can test the stored `position` by printing it. For example, that character 'e' is at position 4 in the alphabet.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 7
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)
print(position)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

You should see the position in the alphabet of the character you entered.

--- /task ---

--- task ---

To encrypt the `character`, you should add the `key` to the `position`. This is then stored in a variable called `new_position`.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 9-10
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)
print(position)

new_position = position + key
print(new_position)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

As your `key` is 3, it should add 3 to the `position` and store it in your `new_position` variable.

For example, letter 'e' is at position 4. To encrypt, you add the `key` (3), giving 7.

```
Please enter a character: e
4
7
```

--- /task ---

--- task ---

What happens when you try and encrypt the letter 'y'?

```
Please enter a character: y
24
27
```

Notice how the `new_position` is 27, and there aren't 27 letters in the alphabet!

--- /task ---

--- task ---

Use a `%` to tell the new position to go back to position 0 once it gets to position 26.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 9
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)
print(position)

new_position = (position + key) % 26
print(new_position)
--- /code ---

--- /task ---

--- task ---

Finally, print the letter at the new position.

For example, adding the key to the letter 'e' gives 7, and the letter at position 7 of the alphabet is 'h'.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 12-13
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)
print(position)

new_position = (position + key) % 26
print(new_position)

new_character = alphabet[new_position]
print(new_character)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

Try out your code. 

--- /task ---

--- task ---

Remove some of your print statements, just printing the new character at the end.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 11
---
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26

new_character = alphabet[new_position]
print('The new character is: ', new_character)
--- /code ---
--- /task ---

--- task ---

**Test:** Click the **Run** button and try out your program!

--- /task ---
