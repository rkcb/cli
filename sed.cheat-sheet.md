
# Basic commands

  - # comment
  - q # exit code e.g.  seq 3 | sed 2q
  - d # Delete the pattern space; immediately start next cycle.
      # example  seq 3 | sed 2d
  - p # print the pattern space
  - n # If auto-print is not disabled, print the pattern space, then, regardless, replace
      # the pattern space with the next line of input. If there is no more input then
      # sed exits without processing any more commands.



  - substitute only one command => sed 's/esa/escobar/'
  -
 
  ## Addresses

    1. No address => apply command to all lines
    2. Exactly one address => apply only to all lines that match the address
    3. Negate an address with !

  ### Examples 

    1. replace  x with y in the line 3 => sed '3s/x/y'
    2. address range; do a replace in the lines 1-3 x's with y's => sed '1,3s/x/y/g'
    3. replace x's with y's if line does contain w => sed 'w!s/x/y/g'
    4. insert note to the first line => sed -i '1 inote' myfile.txt

# POSIX Character classes
	
[:alnum:]
Alphanumeric characters: ‘[:alpha:]’ and ‘[:digit:]’; in the ‘C’ locale and ASCII character encoding, this is the same as ‘[0-9A-Za-z]’.

[:alpha:]
Alphabetic characters: ‘[:lower:]’ and ‘[:upper:]’; in the ‘C’ locale and ASCII character encoding, this is the same as ‘[A-Za-z]’.

[:blank:]
Blank characters: space and tab.

[:cntrl:]
Control characters. In ASCII, these characters have octal codes 000 through 037, and 177 (DEL). In other character sets, these are the equivalent characters, if any.

[:digit:]
Digits: 0 1 2 3 4 5 6 7 8 9.

[:graph:]
Graphical characters: [:alnum:] and [:punct:].

[:lower:]
Lower-case letters; in the ‘C’ locale and ASCII character encoding, this is a b c d e f g h i j k l m n o p q r s t u v w x y z.

[:print:]
Printable characters: ‘[:alnum:]’, ‘[:punct:]’, and space.

[:punct:]
Punctuation characters; in the ‘C’ locale and ASCII character encoding, this is ! " # $ % & ' ( ) * + , - . / : ; < = > ? @ [ \ ] ^ _ ` { | } ~.

[:space:]
Space characters: in the ‘C’ locale, this is tab, newline, vertical tab, form feed, carriage return, and space. See Usage, for more discussion of matching newlines.

[:upper:]
Upper-case letters: in the ‘C’ locale and ASCII character encoding, this is A B C D E F G H I J K L M N O P Q R S T U V W X Y Z.

[:xdigit:]
Hexadecimal digits: 0 1 2 3 4 5 6 7 8 9 A B C D E F a b c d e f.


