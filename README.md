# python_week4_Assignment

# Read the contents of input.txt
input_file_path = "g:\\Software Engineering\\Python\\input.txt"
output_file_path = "g:\\Software Engineering\\Python\\output.txt"

with open(input_file_path, "r") as input_file:
    content = input_file.read()

# Count the number of words in the file
word_count = len(content.split())

# Convert all text to uppercase
uppercase_content = content.upper()

# Write the processed text and the word count to output.txt
with open(output_file_path, "w") as output_file:
    output_file.write(uppercase_content)
    output_file.write("\n\n")
    output_file.write(f"Word Count: {word_count}")
