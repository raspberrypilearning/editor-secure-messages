## Encrypt the character

Print the `position` of the character.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="5-7"
alphabet = 'abcdefghijklmnopqrstuvwxyz'

character = input('Please enter a character: ')

position = alphabet.find(character)

print(position)
```

> [!TIP]
>
> - The letter `a` is at position `0` in the alphabet

## Now run your code

Run your code, enter a character, and check that its position in the alphabet is printed.

```
Please enter a character: 
e
4
```
