# pig
'''
RULES:
if a word starts with a  vowel,add 'ay' to end.
if a word does not start with a vowel, put first letter at the end , then add 'ay'.
for eg:
    word= ordway
    apple= appleay  
'''
def pig_latin(word):
    first_letter= word[0]

    if first_letter in 'aeiou':
        pig_word= word +'ay'

    else:
        pig_word= word[1:] + first_letter+ 'ay'

    return pig_word
for word in range(7):
    word= str(input("enter the string "))
    print(pig_latin(word))
