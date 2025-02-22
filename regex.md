1) 
import re
def function(string):
      patterns = r'^ab*$'
    if re.match(patterns, string):
        return "True"
    else:
        return "False"

print(function("a"))
print(function("abc"))  
print(function("abb"))   
print(function("aaab"))  
print(function("abab"))   


2)
import re
def function(string):
    patterns = 'ab{2,3}?'
    if re.match(patterns, string):
        return "True"
    else:
        return "False"

print(function("a"))
print(function("abc"))  
print(function("abb"))   
print(function("aaab"))  
print(function("abab")) 


3)
import re
def function(string):
    patterns = r'[a-z]+(?:_[a-z]+)+' 
    matches = re.findall(patterns, string)
    return matches
string1 = "hello_w how are_you"
result = function(string1)
print(result)


4)
import re
def function(string):
    patterns = r'[A-Z][a-z]+'
    matches = re.findall(patterns, string)
    return matches
string1 = "Hello how are You"
result = function(string1)
print(result)


5)
import re
def function(string):
    patterns = r'\ba[a-z]*b\b'
    matches = re.findall(patterns, string)
    return matches
string1 = "alnfghb how are You"
result = function(string1)
print(result)
