
# Examples of Linux find command usages

1. Find all files contained in the current directory or its subdirectory:

find /home/escobar notes.txt

Empty path means current directory.

2. Find files using wild cards and case insensitivity

find /home/escobar -iname "\*.php"

(-name if case sensitivity is desired)

3. Limit the search depth

find . -maxdepth 2 -name \*.java

4. Negate th match

find . -not -name \*.php

find . ! -name \*.php

5.  Combine the search criteria with a negation

find . -name \*.php ! 

6. As above but 'or'

find . -name \*.php -o -name \*.js

7. Find only files 

find . -name file.txt -type f 

8. Find only directories 

find . -name file.txt -type d 



