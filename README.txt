First   BFA   topics 
Python   basics 
Clean   c   ode 
Naming   conventions,   clean   code   DOs   and   DON’Ts   (indentation,   comments,   do   not   name   2 
variables/function   the   same   way,   no   code   outside   functions,   meaningful   names,   always 
use   English,   use   globals   only   if   needed) 
Using   v   ariables  
Variable   types,   variable   operations.   Immutable   vs.   mutable,   passing   by   value   and 
reference.   Casting   variables   ­   when/why.   Meaning   of   NameError:   XXX   is   not   defined. 
Scope   o
  f   v   ariables 
Global   vs   function   scope.   How   to   read/write   a   global   variable? 
Loops,   c   ontrol   s   tatements,   o
  perators 
for   and   while   (break,   continue),   if­elif­else.   Single   line   control   statements  
Operators:   not,   or,   and,   >,   <,   >=,   <=,   ==,   !=,   %   (modulo),   //,   +,   ­,   *,   / 
Operators   and   types   (  most     operators   are   defined   for   the   same   type). 
Subscript   operator,   []. 
Functions/Methods 
How   to   define   them,   input   parameters,   return   values.   Advanced:   Call   stack.  
Built in data structures 

Lists/Arrays:   
How   to   add element:
my_list.append("string")
    
Remove elements:


mylist = [[1, 2, 3], [4, 5, 6, 7], [8, 9, 10]]
"""
for element in mylist:
    if len(element) == 3:
        print(element)


for index in range(len(mylist)):
    if len(mylist[index]) == 3:
        print(mylist[index])
"""

print(mylist)
#érték szerint megadva törli a lista elemét
mylist.remove([1,2,3]) 
print(mylist)
#index szerint megadva törli a lista elemét
mylist.pop(0)



lists,   sorting


Dictionaries:   
What are keys, values, how to check if it contains an element. 
if key in dictionary:   #kell a . keys?

Retrieve an element by a key.
dictionary["ember"]

dictionary = {"ember" : 10, "allat" : 5, "haz" : 2}

for key, value in dictionary.items():
    print(key, value)

for key in dictionary.keys():
    print(key)

for value in dictionary.values():
    print(value)

Tuples:   Immutable  

Built in primitive types 
Strings: Are immutable 

Search:
str1 = "this is final exam!!!"  
str2 = "exam" 

print(str1.find(str2))
print(str1.find(str2, 10))
print(str1.find(str2, 20))

Get substring (slice):
 s = 'Hello, everybody!'
>>> s[0]
'H'
>>> s[:3]
'Hel'
>>> s[2:5]

.split()
.strip()

Length:
len(string)

Strings as lists. 

Numbers: int, float 

Built in methods:
Print:

Input:
input()

Range:  
#generátor függvény
számsorozatot állít elő
range(start, stop[, step])

Random:
import random

random.randint(0,100) #itt benne van a 0 és a 100 is
random.randrange(start, stop[, step])  #itt lépészámot is lehet megadni, de nincs benne a végpont
random.random() #fixen 0 és 1 között floatot generál


File   I/O:
# file-ból olvas, listába tölt
my_file = open("testfile.txt", "r")
output_list = []
for line in my_file:
    output_list.append(line)
my_file.close()


# file-ba ír, lista elemeit soronként
my_file = open("testfile.txt", "w")
for line in output_list:
    my_file.write(line + "\n")
my_file.close()


#With statement, bezárja magát:
file_name = "testfile.txt"
output_list = []

with open(file_name, "r") as data_file:
    for line in data_file:
        output_list.append(line)

with open(file_name, "w") as data_file:
    for element in output_list:
       data_file.write(element + "\n")



Debugging/testing your code.
Using print statements, (advanced) debugging via VS Code, breakpoints.  


GIT 
Usage   in   terminal: 
git log – naplózza a commitokat 
git status
man git-<parancs neve>
touch mate.py
rm mate.py

ctrl + z -lerakja háttérbe a futó processt
jobs  -kilistázza a futó alkalmazásokat
fg  -visszahozza az utolsó háttérbe rakott alkalmazást
fg 1 vagy fg 2 vagy stb (azt hozza be, ahol a + jel van)
nano-ban ctrl + O a mentés

Create a repo:
mkdir folder
cd folder
git init
touch mate.py -létrehoz python file
git add . (vagy file neve)
git commit (git commit -m “ szöveg“
git commit --amend -újra megcsinálja az utlosó commitot
git remote add origin <repo URL>
git push origin master  -hova mit
>>> s[0]

Clone   a   repo:
git clone <URL name>

Pull,   add,   commit,   push. 
Best   practices   (commit   messages,   do   not   use   file   upload!,   always   pull   before   push) 
Advanced:   How   to   handle   merge   conflict   (no   need   to   do   Git   merge,   just   do   something   that 
works,   e.g.   Git   reset,   then   push   your   changes) 
 
