
# Loops 

- for ([initialExpression]; [condition]; [incrementExpression])
- do { } while ()
- the for...in statement iterates over all non-Symbol, enumerable properties of an object.
    * example: for (var property1 in object1) {}
    * use for debugging purposes only
- for (variable of object) {}
    * use with iterable objects (including Array, Map, Set, arguments object and so on)

# Strings

- template string => `value = ${myvar}`
- replace text with a regexp or text => str.replace(/myold/gi, 'mynew') 
-
-

# Serialization

- functions are never serialized 
- regular expressions are not serialized by JSON.stringify
- 
