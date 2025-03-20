Print all the duplicates in the input string
------------------------------------------------------------------

def print_duplicates(input_string):
    duplicates = {}
    for char in input_string:
        duplicates[char] = duplicates.get(char, 0) + 1
    print("Duplicates:")
    for char, count in duplicates.items():
        if count > 1:
            print(f"{char} appears {count} times")
input_string=str(input())
print_duplicates(input_string)
