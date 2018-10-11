# 6.18.1
def get_num_of_characters(inputStr):
    characters = 0
    for letter in inputStr:
        characters += 1
    return characters

def output_without_whitespace(inputStr):
    output='';
    for letter in inputStr:
        if letter !='\t':
            output += letter
    return output


if __name__ == '__main__':
    inputStr = input('Enter a sentence or phrase:')
    print()
    print()
    print('You entered:', inputStr)
    print()
    
    characters = get_num_of_characters(inputStr)
    print('Number of characters:', characters)
    no_whitespace = output_without_whitespace(inputStr)
    print('String with no whitespace:', no_whitespace)
