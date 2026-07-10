## Encrypt a full message

Store the user's message and use a `for` loop to repeat the code for each character in the message.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="5-13"
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = input('Please enter the key: ')
key = int(key)

message = input('Please enter a message: ')

for character in message:
	position = alphabet.find(character)

	new_position = (position + key) % 26

	new_character = alphabet[new_position]
	print('The new character is: ', new_character)
```

## Now run your code

Run your code, enter a message, and check that a new encrypted character is printed for each letter.

```
Please enter the key: 5
Please enter a message: hello
The new character is:  m
The new character is:  j
The new character is:  q
The new character is:  q
The new character is:  t
```
