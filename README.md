# valid_pilandrome
A phrase is a palindrome if, after converting all uppercase letters into lowercase letters and removing all non-alphanumeric characters, it reads the same forward and backward. Alphanumeric characters include letters and numbers.

class Solution:
    def isPilandrome(self, s:str) -> bool:
        # create a new string that will take only letters or numbers
        word = ''
        
        # iterate through the string and filter out non-alphabet or non-numerical and add it in the word variable
        for char in s:
            # convert each character into lower case
            char_lowered = char.lower()
            if char_lowered.isalpha() or char.isdigits == True:
                word += char_lowered
                
            # compare word and reversed word and return the result 
            return word == word[::-1]
