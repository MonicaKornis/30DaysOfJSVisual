##Day 2

## Primitive VS Non-Primitive Data Types 

Primitive Data Types in Javascript 
* Numbers - Ints, Floats
* Strings
* Booleans
* Null 
* Undefined
* Symbol



Non-Primitive Data Types in Javascript 
* Objects 
* Arrays


Also in Javscript, if it's not a primitive data type it's actually secretly an object 🤫

What's the difference between these data types? Immutability - which is just a fancy way of saying that they cannot be changed once they are created.  

There are many instances where it may appear like you can modify the values of these data types. However, that's not what is happening under the hood. One example of this is when you add a character to the end of aa string. It appears like the value itself is being changed, yet that is not actually what is happening. In reality, a new string is getting created with the new character character at the end. That string then get allocated to a new location in memory and the system points the variable to the new value. 

Non-primitive data types, on the other hand, can be modified or changed. They also cannot be compared by value, even when the properties in an object or array are the same: 

```
 [1,2,4] == [1,2,4] // false 
```

Therefore, as a rule of thumb, we do not compare non-primitive data types. Non-primitive data types are one equal when they point to the same underlying object. 

## Numbers 

The Math object provides a lot of useful methods to help us work with numbers

* Math.round()
* Math.min(-5, 3, 20, 4, 5, 10) //20
* Math.max(-5, 3, 20, 4, 5, 10) //-5
* Math.ceil (4.623) // 5
* Math.random() * 10 // creates random number between 0 to 0.999999
* Math.pow(3,2) // 3 to the second power = 9 

* Math.ceil(Math.random() * 10) //generates a random number between 1 and 10
* Math.floor(Math.random() * (100 - 50 + 1)) + 50 // generates a random number between 50 and 100
* How to shuffle an array using Math.random: const shuffledArray = array.sort((a, b) => 0.5 - Math.random());

Escape Sequences in Javascript 

* \n: new line
* \t: Tab, means 8 spaces
* \\: Back slash
* \': Single quote (')
* \": Double quote (") 

```
"This is Monica\`s house"
'My mother once said \"Eat your vegetables\"'
```

## Strings 

* substring(start, end) returns a substring starting at the first argument and up until (excluding) the second argument 
    'string'.substring(1,3) ---> 'tr'
* trim()  removes the empty space characters at the beginning and end of a string 
* replace(substring1, substring2) replaces the first argument with the second argument in the string 
    ex: 'stringgg'.replace('ggg', 'sss')  ---> 'strinsss'
* startsWith(substr): returns a boolean if string starts with the argument provided
* endssWith(substr): returns a boolean if string ends with the argument provided
* search(substring): takes in a substring and returns the index of it's first match


## Data Types 

* You can check the data type of a value with the typeof method 

Casting or Changing the Data Type 

Ways to change a string to an int: 
* parseInt()
* Number()
* Plus sign(+)

Ways to change a string to a float: 
* parseFloat()
* Number()
* Plus sign(+)

Ways to change a float to an int: 
* parseInt()