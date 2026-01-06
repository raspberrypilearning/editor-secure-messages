<h2 class="c-project-heading--task">Handle special characters</h2>
--- task ---
Only translate a character if it's in the alphabet. 
--- /task ---

Add an `if` `else` statement to your code, which only encrypts alphabet charcaters and adds the original special character to the encrypted message.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 9
line_highlights: 10-18
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
</div>

<div class="c-project-output">
<pre>Please enter the key: 5
Please enter a message: hello!!
mjqqt!!</pre>
</div>
