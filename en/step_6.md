## Extra characters

Some characters are not in the alphabet, which causes an error.

--- task ---

Test out your code with some characters that are not in the alphabet.

For example, you could use the message `hi there!!`.

```
Please enter a message: hi there!!
klcwkhuhcc
```

Notice that the space and the `!` characters are all encrypted as the letter 'c'!

--- /task ---

--- task ---

To fix this, only translate a character if it's in the alphabet. To do this, add an `if` statement to your code, and indent the rest of your code.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 8
line_highlights: 9
---
for character in message:
    if character in alphabet:
    	position = alphabet.find(character)
    
    	new_position = (position + key) % 26
    
    	new_character = alphabet[new_position]
    
    	new_message += new_character
print(new_message)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button and test with the same message. 

What happens this time?

```
Please enter a message: hi there!!
klwkhuh
```

Your code just skips any character if it is not in the alphabet.

--- /task ---

It would be better if your code just used the original character for anything not in the alphabet.

--- task ---

Add an `else` statement to your code, which just adds the original character to the encrypted message.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 8
line_highlights: 17-18
---
for character in message:
    if character in alphabet:
    	position = alphabet.find(character)
    
    	new_position = (position + key) % 26
    
    	new_character = alphabet[new_position]
    
    	new_message += new_character
    else:
        new_message += character
print(new_message)
--- /code ---

--- /task ---

--- task ---

**Test:** Click the **Run** button. 

You should see that any character in the alphabet is encrypted, but any other characters are left alone!

```
Please enter a message: hi there!!
kl wkhuh!!
```
--- /task ---
