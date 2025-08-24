"""
File Read & Write Challenge 🖋️
This program reads a file, modifies its content, and writes it to a new file.
It also includes error handling if the file does not exist or cannot be read.
"""

def read_and_modify_file(input_filename, output_filename):
    try:
        # Open the input file for reading
        with open(input_filename, "r") as infile:
            content = infile.read()

        # Modify the content (example: make it uppercase)
        modified_content = content.upper()

        # Write the modified content to a new file
        with open(output_filename, "w") as outfile:
            outfile.write(modified_content)

        print(f"✅ Successfully created '{output_filename}' with modified content.")

    except FileNotFoundError:
        print(f"❌ Error: The file '{input_filename}' was not found.")
    except PermissionError:
        print(f"❌ Error: Permission denied for file '{input_filename}'.")
    except Exception as e:
        print(f"⚠️ Unexpected error: {e}")


if __name__ == "__main__":
    # Ask the user for a filename
    input_file = input("Enter the name of the file to read: ")
    output_file = "modified_" + input_file

    read_and_modify_file(input_file, output_file)
