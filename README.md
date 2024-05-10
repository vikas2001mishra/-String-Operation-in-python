# String-Operation-in-python

# string methods :
         lower(): Converts all uppercase characters in a string into lowercase
         upper(): Converts all lowercase characters in a string into uppercase
         title(): Convert string to title case
         swapcase(): Swap the cases of all characters in a string
         capitalize(): Convert the first character of a string to uppercase


# Method	Description :

# capitalize()	Converts the first character to upper case
# casefold()	Converts string into lower case
# center()	Returns a centered string
# count()	Returns the number of times a specified value occurs in a string
# encode()	Returns an encoded version of the string
# endswith()	Returns true if the string ends with the specified value
# expandtabs()	Sets the tab size of the string
# find()	Searches the string for a specified value and returns the position of where it was found
# format()	Formats specified values in a string
# format_map()	Formats specified values in a string
# index()	Searches the string for a specified value and returns the position of where it was found
# isalnum()	Returns True if all characters in the string are alphanumeric
# isalpha()	Returns True if all characters in the string are in the alphabet
# isascii()	Returns True if all characters in the string are ascii characters
# isdecimal()	Returns True if all characters in the string are decimals
# isdigit()	Returns True if all characters in the string are digits
# isidentifier()	Returns True if the string is an identifier
# islower()	Returns True if all characters in the string are lower case
# isnumeric()	Returns True if all characters in the string are numeric
# isprintable()	Returns True if all characters in the string are printable
# isspace()	Returns True if all characters in the string are whitespaces
# istitle()	Returns True if the string follows the rules of a title
# isupper()	Returns True if all characters in the string are upper case
# join()	Converts the elements of an iterable into a string
# ljust()	Returns a left justified version of the string
# lower()	Converts a string into lower case
# lstrip()	Returns a left trim version of the string
# maketrans()	Returns a translation table to be used in translations
# partition()	Returns a tuple where the string is parted into three parts
# replace()	Returns a string where a specified value is replaced with a specified value
# rfind()	Searches the string for a specified value and returns the last position of where it was found
# rindex()	Searches the string for a specified value and returns the last position of where it was found
# rjust()	Returns a right justified version of the string
# rpartition()	Returns a tuple where the string is parted into three parts
# rsplit()	Splits the string at the specified separator, and returns a list
# rstrip()	Returns a right trim version of the string
# split()	Splits the string at the specified separator, and returns a list
# splitlines()	Splits the string at line breaks and returns a list
# startswith()	Returns true if the string starts with the specified value
# strip()	Returns a trimmed version of the string
# swapcase()	Swaps cases, lower case becomes upper case and vice versa
# title()	Converts the first character of each word to upper case
# translate()	Returns a translated string
# upper()	Converts a string into upper case
# zfill()	Fills the string with a speci


# Example 1:


city = input("Enter Your City Name:")
list = ['Prayagraj','Lucknow','Varanasi','Bhadohi']
if city in list:
    print("Your City is available")
else:
    print("Your city is not available")



'''s = 'VikasMishraVikasMishra'
print(s.find('Mishra'))'''



'''s = 'VikasMishraVikasMishra'
print(s.find('Sharma'))'''         # if the value is not present output will be always  -1.



'''s = 'VikasMishraVikasMishra'
print(s.find('Mishra',7,22))'''





# rfind() --> reverse direction.

s = 'VikasMishraVikasMishra'
print(s.rfind('Mishra'))
print(s.index('Mishra'))  #index()
print(s.index('Mishra',7,22))
print(s.rindex('i'))



# try and except:-
# try - The try block lets you test a block of code for errors.
# except - The except block lets you handle the error.



s= input("Enter main string: ")
sub = input("Enter substring: ")
try:
    n=s.index(sub)
except ValueError:
    print('substring is not found in the main string')
else:
    print('substring found')'''

# counting the substring in given string

'''s = 'VikasmishraVikasmishraVikas'
print(s.count('Vikas'))
print(s.count('Vikas',3,22))'''



# replace

'''s='vikasmishravikasmishra'
print(s.replace('vikasmishra','sagartomar'))
print(s.replace('vikas','sagar'))'''






# split

'''s = 'Rohan Mohan Shyam Mishra Sharma Pandey'
list = s.split()
print(list)'''

'''s = 'Rohan-Mohan-Shyam-Mishra-Sharma-Pandey'
list = s.split('-')
print(list)'''

'''s = 'Rohan Mohan Shyam Mishra Sharma Pandey'
list = s.split()
for i in list:
    print(i)'''


'''s = 'vikas mishra prayagraj uttar pradesh'
list = s.split(' ',3)
for i in list:
    print(i)'''




# join

Team = ['Sagar','Shubh','Rakesh','Vikas']
# s = ''.join(Team)
s = '+'.join(Team)
#s = '-'.join(Team)
print(s)



# Some Important:-


s = 'Ram is a good boy'
print(s.upper())
print(s.lower())
print(s.split())
print(s.count('Ram'))
print(s.swapcase())
print(s.index('is'))
print(s.rindex('boy'))
print(s.rfind('is'))
print(s.capitalize())
print(s.title())




# checking starting and ending part of the string


s = 'Mohan is great person'
print(s.startswith('Mohan'))
print(s.endswith('great'))

# isalnum(alpha+numberr both) & it always give "True".

print('Vikas123'.isalnum())
#isalpha()
print('Vikas'.isalpha())
print('1234'.isalpha())
#isdigit()
print('9876'.isdigit())
print('abcd'.isdigit())
#islower()
print('vikas'.islower())
print('Vikas'.islower())
#isupper()
print('vikas'.isupper())
print('VIKAS'.isupper())
#istitle()
print('vikas'.istitle())
print('Vikas'.istitle())
#isspace()
print('vikas mishra'.isspace())
print(' '.isspace())




'''s = input("Enter any character:")
if s.isalnum():
    print("Alpha numeric character")
    if s.isalpha():
        print("Alphabet character")
        if s.lower():
            print("Lower case Alphabet character")
        else:
            print("upper case Alphabet character")
    else:
        print("It's Digit")
elif s.isspace():
    print("it's a space character")
else:
    print("none space special character")'''




# Reverse Direction

s = "Rahul"
print(s[::-1])


'''s = input("Enter the string:")
print(s[::-1])'''

# Slicing:
  #Slicing is the extraction of a part of a string, list, or tuple.


s = input("Enter some string:")
print("character at position",s[::2])
print("character at position",s[1::2])


