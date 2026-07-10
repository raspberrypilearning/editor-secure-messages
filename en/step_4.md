## Wrap around

Use a `%` to make `new_position` reset to 0 once it gets to 26.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="8"
alphabet = 'abcdefghijklmnopqrstuvwxyz'
key = 3

character = input('Please enter a character: ')

position = alphabet.find(character)

new_position = (position + key) % 26
print(new_position)
```

> [!DEBUG]
>
> - Make sure you have brackets around `position + key`

## Now run your code

Run your code, enter a character at the end of the alphabet, such as `y`, and check that the position wraps back to the start of the alphabet.

```
Please enter a character: y
1
```
