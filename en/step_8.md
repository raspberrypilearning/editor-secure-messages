## Print the new message on one line

Store the new message in a variable, add each new character to it and print it at the end.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="4,15,16"
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
```

## Now run your code

Run your code, enter a message, and check that the full encrypted message is printed as one word.

```
Please enter the key: 5
Please enter a message: hello
mjqqt
```
