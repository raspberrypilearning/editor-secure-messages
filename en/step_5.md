## Print the letter at the new position

Output the character at the new position.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="11-12"
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26
print(new_position)

new_character = alphabet[new_position]
print(new_character)
```

## Now run your code

Run your code, enter a character, and check that the encrypted letter is printed.

```
Please enter a character: e
7
h
```
