# ASCII Value Checker

print("ASCII Value Checker")

print("="* 40)

# Get input from user
char = input("Enter a character: ")

if type(char) is str and len(char) ==1:
    # get ASCII value

    ascii_value = ord(char)
    print(f"\n Character: '{char}'")
    print(f"ASCII Value: {ascii_value}")

    # identify type
    print("\nCharacter Type:",end="")

    if ascii_value >= 65 and ascii_value <= 90:
        print("Uppercase Letter")
    elif ascii_value >= 97 and ascii_value <= 122:
        print("Lowercase Letter")
    elif ascii_value >= 48 and ascii_value <= 57:
        print("Digit")
    elif ascii_value == 32:
        print("Space")
    else:
        print("Special Character")

else:
    print("Invalid input. Please enter a single character.")
