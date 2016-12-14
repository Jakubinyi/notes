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
Built   i   n   d
  ata   s   tructures 
Lists/Arrays:   How   to   add,   remove   elements,  
lists,   sorting 
Dictionaries:   What   are   keys,   values,   how   to   check   if   it   contains   an   element.   Retrieve   an 
element   by   a   key 
Tuples:   Immutable  
Built   i   n   p
  rimitive   t   ypes 
Strings:   Are   immutable,   search,   get   substring   (slice),   length,   strings   as   lists. 
Numbers:   int,   float Built   i   n   m
  ethods 
Print,   input,   range,   random,   

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



Debugging/testing   your   code.
Using   print   statements,   (advanced)   debugging   via   VS   Code,   breakpoints.  


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


Clone   a   repo:
git clone <URL name>

Pull,   add,   commit,   push. 
Best   practices   (commit   messages,   do   not   use   file   upload!,   always   pull   before   push) 
Advanced:   How   to   handle   merge   conflict   (no   need   to   do   Git   merge,   just   do   something   that 
works,   e.g.   Git   reset,   then   push   your   changes) 
 
