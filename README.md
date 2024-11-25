- 👋 Hi, I’m @laddumuthya
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
def reverse_string(s):
    return s[::-1]


def change_case(s):
    return s.swapcase()


def count_vowels(s):
    vowels = "aeiouAEIOU"
    count = sum(1 for char in s if char in vowels)
    return count


def is_palindrome(s):
    return s == s[::-1]


def main():
    print("Welcome to the String Manipulation Program!")
    while True:

        user_string = input("Enter a string (or type 'exit' to quit): ")
        if user_string.lower() == 'exit':
            print("Exiting the String Manipulation Program. Goodbye!")
            break

        print("\nChoose an operation:")
        print("1. Reverse the string")
        print("2. Change case")
        print("3. Count vowels")
        print("4. Check if palindrome")
        print("5. capitalize the string")
        print("6: convert string to lowercase")
        print("7: convert string to uppercase")
        print("8: Center")
        print("9: Endswith")
        print("10: Identify whether string is made up of all digits or not")
        print("11. Strip")
        print("12. Count characters")
        print("13. Check to see if it is ASCII")
        print("14. All of the above")

        choice = input("Enter your choice (1-14): ")

        if choice == '1':
            print(f"Reversed String: {reverse_string(user_string)}")

        elif choice == '2':
            print(f"Changed Case: {change_case(user_string)}")

        elif choice == '3':
            print(f"Number of Vowels: {count_vowels(user_string)}")

        elif choice == '4':
            palindrome_result = "Yes" if is_palindrome(user_string) else "No"
            print(f"Is Palindrome: {palindrome_result}")

        elif choice == '5':
            print(f"Capitalize the string: {user_string.capitalize()}")

        elif choice == '6':
            print(f"Convert to lowercase: {user_string.lower()}")

        elif choice == '7':
            print(f"Convert to uppercase: {user_string.upper()}")

        elif choice == '8':
            print(f"String at centre: {user_string.center(15)}")

        elif choice == '9':
            print(f"Yes" if user_string.endswith(".") else "No")

        elif choice == '10':
            print(f"the string is made of digits" if user_string.isdigit() else "string is not full of digits")

        elif choice == '11':
            print(f"Stripped string: {user_string.strip()}")

        elif choice == '12':
            ch = input("Enter character to count: ")
            print(f"Count of your character is: {user_string.count(ch)}")

        elif choice == '13':
            print(f"Is ASCII: {user_string.isascii()}")

        elif choice == '14':
            print(f"Reversed String: {reverse_string(user_string)}")
            print(f"Changed Case: {change_case(user_string)}")
            print(f"Number of Vowels: {count_vowels(user_string)}")
            palindrome_result = "Yes" if is_palindrome(user_string) else "No"
            print(f"Is Palindrome: {palindrome_result}")
            print(f"Capitalize the string: {user_string.capitalize()}")
            print(f"Convert to lowercase: {user_string.lower()}")
            print(f"Convert to uppercase: {user_string.upper()}")
            print(f"String at centre: {user_string.center(25)}")
            print(f"Yes" if user_string.endswith(".") else "No")
            print(f"the string is made of digits" if user_string.isdigit() else "string is not full of digits")
            print(f"Stripped string: {user_string.strip()}")
            ch = input("Enter character to count: ")
            print(f"Count of your character is: {user_string.count(ch)}")
            print(f"Check if it is ASCII: {user_string.isascii()}")

        else:
            print("Invalid choice. Please try again.")


# Run the program
main()
"""bmi"""

def calculate_bmi(weight, height):
    """Calculate the BMI given weight and height."""
    return weight / (height ** 2)
def classify_bmi(bmi):
    """Classify the BMI according to standard ranges"""
    if bmi < 18.5:
        return "Underweight"
    elif 18.5 <= bmi < 24.9:
        return "Normalweight"
    elif 24.9 <= bmi < 29.9:
        return "Overweight"
    else:
        return "Obesity"
def main():
    """Main function to run bmi calculator"""
    while True:
        print("\n BMI Calculator")
        #get user input
        weight = float(input("Enter the weight in kilograms: "))
        height = float(input("Enter the height in meters:"))
        #calculate BMI and classify it
        bmi = calculate_bmi(weight, height)
        category = classify_bmi(bmi)
        #display result
        print(f"your Bmi is: {bmi:.2f}")
        print(f"BMI Category: {category}")
        #ask if user wants to calculate again
        choise = input("Do you want to calculate another BMI ? (Y/N): ")
        if choise.lower() == "y":
            print("Exiting Bmi Calculator stay healthy")
            break

main()
<!---
laddumuthya/laddumuthya is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
