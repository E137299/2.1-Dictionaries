# 2.1-Dictionaries

# Student Dictionaries

### Instructions:
1. **Creating a Dictionary:**
    - Create a dictionary called student_info that contains the following key-value pairs:
        - "name": Your name (as a string)
        - "age": Your age (as an integer)
        - "grade": Your current grade (as a string, e.g., "A", "B", "C")
        - "subjects": A list of subjects you are currently taking (as a list of strings)
        - "is_full_time": A boolean value indicating whether you are a full-time student (True or False)
2. **Accessing Values:**

    - Print the value associated with the "name" key from the student_info dictionary.
    - Print the value associated with the "grade" key.
    - Print the list of subjects you are taking.
3. **Modifying the Dictionary:**

    - Update the "grade" key to a new value that represents your desired grade at the end of the term.
    - Add a new key-value pair to the dictionary:
        - "favorite_subject": The subject you enjoy the most (as a string).
    - Remove the "is_full_time" key from the dictionary.
4. **Looping Through the Dictionary:**

    - Use a for loop to iterate over the student_info dictionary and print each key and its corresponding value in the format "key: value".
5. **Nested Dictionary:**
    - Add a nested dictionary called "scores" to the student_info dictionary with the following key-value pairs:
        - "Math": A score out of 100 for Math (as an integer)
        - "Science": A score out of 100 for Science (as an integer)
        - "English": A score out of 100 for English (as an integer)
    - Print the score for Math.

### Example Output:
```python
John
B
['Math', 'Science', 'English']

Updated grade: A
Updated dictionary: {'name': 'John', 'age': 20, 'grade': 'A', 'subjects': ['Math', 'Science', 'English'], 'favorite_subject': 'Science', 'scores': {'Math': 95, 'Science': 88, 'English': 92}}

Key: name, Value: John
Key: age, Value: 20
Key: grade, Value: A
Key: subjects, Value: ['Math', 'Science', 'English']
Key: favorite_subject, Value: Science
Key: scores, Value: {'Math': 95, 'Science': 88, 'English': 92}

Math score: 95
```
**Bonus Challenge:**

Add a feature to your code that calculates and prints the average score of the subjects in the "scores" dictionary.

<br></br>
<br></br>
# Managing a Phone Contact List

## Instructions:
1. **Creating the Contact List:**
    - Create an empty dictionary called *contact_list* that will store contact names as keys and their phone numbers as values.
2. **Adding a New Contact:**
    - Write a function *add_contact(contact_list, name, number)* that takes the *contact_list* dictionary, a contact name (string), and a number (string) as arguments.
    - Inside the function, check if the contact name already exists in the *contact_list*:
    - If it exists, print a message saying "Contact already exists."
    - If it does not exist, add the new contact to the dictionary with the name as the key and the number as the value. Then, print a message saying "Contact added successfully."
3. **Removing a Contact:**
    - Write a function *remove_contact(contact_list, name)* that takes the contact_list dictionary and a contact name (string) as arguments.
    - Inside the function, check if the contact name exists in the *contact_list*:
        - If it exists, remove the contact from the dictionary and print a message saying "Contact removed successfully."
        - If it does not exist, print a message saying "Contact not found."
4. **Viewing the Contact List:**

    - Write a function *view_contacts(contact_list)* that takes the *contact_list* dictionary as an argument and prints out all the contacts in the format "Name: Phone Number".
    - If the contact list is empty, print a message saying "No contacts available."
5. **Testing Your Functions:**
    - Create a test contact list by adding a few contacts using the add_contact function.
    - Attempt to add a contact that already exists to test the duplicate check.
    - Remove a contact using the remove_contact function.
    - View the final contact list using the view_contacts function.

## Example Output:
```python
Adding contacts...
Contact added successfully.
Contact added successfully.
Contact already exists.

Viewing contacts...
Name: Alice, Phone Number: 123-456-7890
Name: Bob, Phone Number: 234-567-8901

Removing a contact...
Contact removed successfully.

Viewing contacts...
Name: Alice, Phone Number: 123-456-7890

Attempting to remove a non-existent contact...
Contact not found.
```
**Bonus Challenge:**
- Enhance the add_contact function to update the existing contact’s number if the contact name already exists, instead of rejecting the addition.
- Write a function find_contact(contact_list, name) that searches for a contact by name and returns the phone number. If the contact is not found, print "Contact not found."