# Python-Programs
Almost 20 Python programs 
1- A program that takes a string as input and counts the number of vowels and consonants in the string.

Input: Hello, World!

Output:

Number of vowels: 3

Number of consonants: 7
2.A Python program that accepts a filename from the user and prints the extension of the file.

Sample filename: document.docx

3.A Python program to check if value 200 exists in the following dictionary.

Sample_dict = {'a': 100, 'b': 200, 'c': 300}

4.The given tuple is a nested tuple. A Python program to print the value 20.

tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))

5.A Python program that calculates the Body Mass Index (BMI) for a person based on their weight (in kilograms) and height (in meters). The BMI is calculated using the following formula:

BMI = (weight) / (height^2)

Instructions:

● Prompt the user to enter their weight in kilograms.

● Prompt the user to enter their height in meters.

● Calculate the BMI using the provided formula.

● Display the calculated BMI to the user.

Additionally, provide an interpretation of the BMI according to the following categories:

● BMI < 18.5: Underweight

● 18.5 <= BMI < 25: Normal weight

● 25 <= BMI < 30: Overweight

● BMI >= 30: Obese

6.A Python program that prompts the user to input a string. The program should count the frequency of each character in the string and then print the result as a dictionary.

EXAMPLE: If the user enters "hello" , the program should output {'h': 1, 'e': 1, 'l': 2, 'o': 1}

indicating that 'h' appears once, 'e' appears once, 'l' appears twice, and 'o' appears once in the input string.

7.Write a Python program that takes a string input from the user and checks if it is a valid email address. If it is valid, print "Valid email address", otherwise print "Invalid email address".

Hint: Check if the string contains “@” and ends with “.net”, or “.com” to check validity. Example: If the email is “abc@example.com”, then it is a valid email, otherwise an Invalid email.
8.Given a tuple of tuples, write a Python program to print the sum of the elements in each inner tuple. (5 marks)

Input: ((1, 2, 3), (4, 5, 6), (7, 8, 9))

Output: 6, 15, 24
9-Create a list containing the 10 numbers . Print the first Three prime numbers from the list.
Expected Output: List of the first three prime numbers: [2, 3, 5]

10.Given a list of dictionaries representing students' information (name, age, grade), Write a Python program to sort the students based on their grades in descending order and print the sorted list.

Dictionary: [

{"name": "John", "age": 20, "grade": 85},

{"name": "Alice", "age": 22, "grade": 90},

{"name": "Bob", "age": 21, "grade": 80} ]

11-Create a program that takes a list of multiple numbers separated with commas (,) from the user and finds the total number of unique values in the list and also prints them.
Expected_format:

Total number of unique values: 6

Unique values in the list: [1, 2, 3, 4, 5, 6]

12.Write a program that takes two lists as input and returns a new list containing elements that are common to both lists.(Hint: Use list methods to implement this.)

Input Lists:

List 1: [1, 2, 3, 4, 5]

List 2: [4, 5, 6, 7, 8]

Common Elements: [4, 5]

13.Write a program that takes two dictionaries as input and merges them into a new dictionary. If there are common keys, combine their values.

dict1= {‘a’:5, ‘b’:10, ‘c’:15}

dict2= {‘b’:20, ‘c’:25, ‘d’:30}

Output: {'a': 5, 'b': 30, 'c': 40, 'd': 30}

14.Write a program that takes two numbers, base and exponent, and calculates the result of raising base to the power of exponent using the ** operator.

Input: Base: 2

Exponent: 3

Result: 8

15.Write a program that takes a temperature in Celsius as input and converts it to Fahrenheit using the formula.

Fahrenheit = (Celsius * 9/5) + 32.


Assignment no 2
1- A program that takes a string as input and counts the number of vowels and consonants in the string.

Input: Hello, World!

Output:

Number of vowels: 3

Number of consonants: 7

[ ]
# create a function
def count_vowels_consonants(text):

# vowels & consonants
  vowels = "aeiou"
  consonants = "bcdfghjklmnpqrstvwxyz"
  vowel_count = 0
  consonant_count = 0

  for x in text.lower():
    if x in vowels:
      vowel_count += 1
    elif x in consonants:
      consonant_count += 1

  return {"vowels": vowel_count, "consonants": consonant_count}
# Get any word from user
text = input("Enter word here : ")
result = count_vowels_consonants(text)
# show output
print(f"Number of vowels: {result['vowels']}")
print(f"Number of consonants: {result['consonants']}")

Enter word here : Hello, World!
Number of vowels: 3
Number of consonants: 7
2.A Python program that accepts a filename from the user and prints the extension of the file.

Sample filename: document.docx

[ ]
# create a function
def get_file_extension(filename):
 # Split the filename by the last dot "."
  parts = filename.split(".")

  # Check if there are parts after the split
  if len(parts) > 1:
    # Return the last part (extension)
    return parts[-1]
  else:
    # No extension found, return empty string
    return ""

# Get the filename from the user
filename = input("Enter a filename: ")

# Get the extension using the function
extension = get_file_extension(filename)

# Print the extension
print("The extension of the file is:", extension)

Enter a filename: document.docx
The extension of the file is: docx
3.A Python program to check if value 200 exists in the following dictionary.

Sample_dict = {'a': 100, 'b': 200, 'c': 300}

[ ]
Sample_dict = {'a': 100, 'b': 200, 'c': 300}

# check if the value 200 exists in the dictionary
if 200 in Sample_dict.values():
  print("Yes, the value 200 exists in the dictinary.")
else:
  print("No, the value 200 does not exist in the dictionary.")
Yes, the value 200 exists in the dictinary.
4.The given tuple is a nested tuple. A Python program to print the value 20.

tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))

[ ]
tuple1 = ("Orange", [10, 20, 30], (5, 15, 25))

# Access the nested list and print the value 20
print(tuple1[1][1])
20
5.A Python program that calculates the Body Mass Index (BMI) for a person based on their weight (in kilograms) and height (in meters). The BMI is calculated using the following formula:

BMI = (weight) / (height^2)

Instructions:

● Prompt the user to enter their weight in kilograms.

● Prompt the user to enter their height in meters.

● Calculate the BMI using the provided formula.

● Display the calculated BMI to the user.

Additionally, provide an interpretation of the BMI according to the following categories:

● BMI < 18.5: Underweight

● 18.5 <= BMI < 25: Normal weight

● 25 <= BMI < 30: Overweight

● BMI >= 30: Obese

[ ]
# create a function
def calculate_bmi(weight, height):
  return weight / height**2

def interpret_bmi(bmi):

  if bmi < 18.5:
    return "Underweight"
  elif 18.5 <= bmi <25:
    return "Normal weight"
  elif 25 <= bmi < 30:
    return "Overweight"
  else:
    return "Obese"
# Get user input
weight = float(input("Enter your weight in kilograms:  "))
height = float(input("Enter your height in meters:  "))

# Calculate and interpret BMI
bmi = calculate_bmi(weight, height)
bmi_interpretation = interpret_bmi(bmi)

print("Your BMI is:", bmi)
print("Interpretation:", bmi_interpretation)




Enter your weight in kilograms:  72
Enter your height in meters:  177
Your BMI is: 0.002298190175237001
Interpretation: Underweight
6.A Python program that prompts the user to input a string. The program should count the frequency of each character in the string and then print the result as a dictionary.

EXAMPLE: If the user enters "hello" , the program should output {'h': 1, 'e': 1, 'l': 2, 'o': 1}

indicating that 'h' appears once, 'e' appears once, 'l' appears twice, and 'o' appears once in the input string.

[ ]
def char_frequency(string):

  char_counts = {}
  for char in string:
    if char in char_counts:
      char_counts[char] += 1
    else:
      char_counts[char] = 1
  return char_counts

# Get string from user
string = input("Enter a string here : ")
char_counts = char_frequency(string)
print(char_counts)  # Output: {'h': 1, 'e': 1, 'l': 2, 'o': 1}

Enter a string here : hello
{'h': 1, 'e': 1, 'l': 2, 'o': 1}
7.Write a Python program that takes a string input from the user and checks if it is a valid email address. If it is valid, print "Valid email address", otherwise print "Invalid email address".

Hint: Check if the string contains “@” and ends with “.net”, or “.com” to check validity. Example: If the email is “abc@example.com”, then it is a valid email, otherwise an Invalid email.

[ ]
# create a function valid email
def valid_email(email):
# Use if else statement and given the all conditions like @, .com,.net

    if '@' in email and (email.endswith('.com') or email.endswith('.net')):
        return True
    else:
        return False
# create another function
def main():
# get input from user
    email = input("Enter an email address: ")
# use if else statement and print output
    if valid_email(email):
        print("Valid email address")
    else:
        print("Invalid email address")

if __name__ == "__main__":
    main()
8.Given a tuple of tuples, write a Python program to print the sum of the elements in each inner tuple. (5 marks)

Input: ((1, 2, 3), (4, 5, 6), (7, 8, 9))

Output: 6, 15, 24

[ ]
# create function
def main():
    input_tuples = ((1, 2, 3), (4, 5, 6), (7, 8, 9))
    result = [sum(inner_tuple) for inner_tuple in input_tuples]
    print("Output:", ', '.join(map(str, result)))

if __name__ == "__main__":
    main()

Create a list containing the 10 numbers . Print the first Three prime numbers from the list.
Expected Output: List of the first three prime numbers: [2, 3, 5]

[ ]
def is_prime(num):

    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True
# Create list of numbers from 1 to 10
numbers = list(range(1, 11))
# Filter prime numbers
prime_numbers = [num for num in numbers if is_prime(num)]
# output
print("List of the first three prime numbers:", prime_numbers[:3])
List of the first three prime numbers: [2, 3, 5]
10.Given a list of dictionaries representing students' information (name, age, grade), Write a Python program to sort the students based on their grades in descending order and print the sorted list.

Dictionary: [

{"name": "John", "age": 20, "grade": 85},

{"name": "Alice", "age": 22, "grade": 90},

{"name": "Bob", "age": 21, "grade": 80} ]

[ ]
# the list of student dictionaries
students = [
    {"name": "John", "age": 20, "grade": 85},
    {"name": "Alice", "age": 22, "grade": 90},
    {"name": "Bob", "age": 21, "grade": 80}
]

# Define a function to sort by grade in descending order
def sort_by_grade(student):
    return student["grade"] * -1

# Sort the list of students using the custom key function
sorted_students = sorted(students, key=sort_by_grade)

# Print the sorted list of students
for student in sorted_students:
    print(f"Name: {student['name']}, Age: {student['age']}, Grade: {student['grade']}")

Name: Alice, Age: 22, Grade: 90
Name: John, Age: 20, Grade: 85
Name: Bob, Age: 21, Grade: 80
Create a program that takes a list of multiple numbers separated with commas (,) from the user and finds the total number of unique values in the list and also prints them.
Expected_format:

Total number of unique values: 6

Unique values in the list: [1, 2, 3, 4, 5, 6]

[ ]
# Get a comma-separated list of numbers from the user
numbers_string = input("Enter a list of numbers separated by commas: ")

# Split the string into a list of numbers
numbers_list = [int(num) for num in numbers_string.split(",")]

# Create a set to efficiently remove duplicates and get unique values
unique_numbers_set = set(numbers_list)

# Print the total number of unique values
print("Total number of unique values:", len(unique_numbers_set))

# Convert the set back to a list to preserve order and print the unique values
unique_numbers_list = list(unique_numbers_set)
print("Unique values in the list:", unique_numbers_list)

12.Write a program that takes two lists as input and returns a new list containing elements that are common to both lists.(Hint: Use list methods to implement this.)

Input Lists:

List 1: [1, 2, 3, 4, 5]

List 2: [4, 5, 6, 7, 8]

Common Elements: [4, 5]

[ ]
def find_common_elements(list1, list2):

    common_elements = []
    for element in list1:
        if element in list2:
            common_elements.append(element)
    return common_elements

# Input lists from the user as coma sepreated
list1 = input("Enter elements of list 1 separated by comma: ").split(',')
list2 = input("Enter elements of list 2 separated by comma: ").split(',')

# Convert input elements to integers (assuming the input is numeric)
list1 = [int(x) for x in list1]
list2 = [int(x) for x in list2]

# Find common elements
common_elements = find_common_elements(list1, list2)

# Output common elements
print("Common Elements:", common_elements)
13.Write a program that takes two dictionaries as input and merges them into a new dictionary. If there are common keys, combine their values.

dict1= {‘a’:5, ‘b’:10, ‘c’:15}

dict2= {‘b’:20, ‘c’:25, ‘d’:30}

Output: {'a': 5, 'b': 30, 'c': 40, 'd': 30}

[ ]
def merge_dicts(dict1, dict2):

    merged_dict = dict(dict1)  # Initialize with dict1 to preserve its contents

    for key, value in dict2.items():
        if key in merged_dict:
            # If the key already exists, add the value to the existing value
            merged_dict[key] += value
        else:
            # If the key is new, simply add it to the merged dictionary
            merged_dict[key] = value

    return merged_dict

# Input dictionaries
dict1 = {'a': 5, 'b': 10, 'c': 15}
dict2 = {'b': 20, 'c': 25, 'd': 30}

# Merge dictionaries
merged_dict = merge_dicts(dict1, dict2)

# Output merged dictionary
print("Merged Dictionary:", merged_dict)

14.Write a program that takes two numbers, base and exponent, and calculates the result of raising base to the power of exponent using the ** operator.

Input: Base: 2

Exponent: 3

Result: 8

[ ]
def power(base, exponent):

    return base ** exponent

# Input base and exponent from the user
base = float(input("Base: "))
exponent = float(input("Exponent: "))

# Calculate result
result = power(base, exponent)

# Output result
print("Result:", result)
15.Write a program that takes a temperature in Celsius as input and converts it to Fahrenheit using the formula.

Fahrenheit = (Celsius * 9/5) + 32.

[ ]
def celsius_to_fahrenheit(celsius):

    fahrenheit = (celsius * 9/5) + 32
    return fahrenheit

# Input temperature in Celsius from the user
celsius = float(input("Enter temperature in Celsius: "))

# Convert Celsius to Fahrenheit
fahrenheit = celsius_to_fahrenheit(celsius)

16.Write a Python program to reverse a list without using built-in functions.

17.Given a string "Hello World", write a Python program to reverse the string without reversing the individual words.

Expected Output: “World Hello”

18-Implement a Python function is_palindrome() that checks whether a passed string is a palindrome (reads the same forward and backward) and tests it with "radar".

19.Write a program that returns a list of even numbers from a given list.

Input: [2, 5, 3, 7, 9, 53, 10, 32, 65, 76, 98]

20.Given two lists keys = ['a', 'b', 'c'] and values = [1, 2, 3], write a Python program to create a dictionary from these lists.

Expected Output: {'a': 1, 'b': 2, 'c': 3}

