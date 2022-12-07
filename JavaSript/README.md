***<h1 align="center">JavaScript</h1>***
# ***Important Links***
<!-- ***[Special](https://html.spec.whatwg.org/multipage/indices.html#element-content-categories)*** -->
## ***Q1. What & What is javaScript?***
*`Brendan Eich` when working at NetScape It was created in 10 days.*

*`JavaScript` improves the user experience of the web page by converting it from a static page into an `interactive` one.*

*JavaScript is a text-based programming language used both on the client-side that allows you to make web pages interactive.*

*Javascript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else.*

*JavaScript is an interpreted language It means it doesn't need a compiler It executes instructions directly without compiling. It is platform independence, dynamic typing The source code is evaluated just before executing it. It is open-source and cross-platform compatible. It is created by NetScape .It has object-oriented capabilities*

## ***Q2. Why JavaScript was developed?***
* *Earlier there was only HTML and CSS were there to build applications, there applications were static*

* *Static applications are the ones in which you cannot take in any user’s input and make some changes in styling or structure of application, so we needed to make the applications dynamic.*

* *Dynamic applications are the ones in which you can take user’s data and save his information. And capturing data is the most important part of the application development.*

## ***Q3. History of JavaScript?***
* *In 1990s, at the time of internet when Microsoft Internet Explorer and Netscape’s Navigator were getting released.*
* *One of the Netscape’s developer named Brandan Eich developed JS in 10 days.*
* *JS used to known as Mocha , then it used to get called as Livescript and then finally Javascript.*
* *Javascript used to get confused with JAVA, but on the other hand they have nothing in common, Javascript is an interpreted language and Java is a compiler language.*
* *Because of all this confusion and to maintain proper standardization in Javascript, Netscape introduced a body called ECMA (European Computer Manufacturers Association)*

## ***Q4. Complier VS Interpreter.***
| COMPILER                              | INTERPRETER                                |
| ------------------------------------- | -------------------------------------------|
| It takes an entire program at a time. | It takes a single line of a code at a time.|
| Compilation is done before execution  | Compilation and Execution takes place simultaneously.|
| Faster because it translates the complete code at one go. | Slower because it translates each line and then execution happens which at last takes more time than compiler|
|It requires memory because it create object code | It does not require any memory.|
| Display all errors at the last. | Display errors after each line if exists.|
| C, C++ | Python, PHPD |

## ***Q5. Add JavaScript in HTML Page.***
* *We can use script tag in `<body>` tag of HTML file.*
* *This script tag should be placed at the end of body tag means after complete HTML code.*
* *`<script src=“./index.js”></script>`*

## ***Q6. Variables in Javascript.***
*Variables are containers. They store data values For ex: var Variables are containers They store data values For ex: var x = 5*

*5 is the value stored in variable x In programming, just like in mathematics, we use variables to hold values x = 5*
```javascript
    var name = 'Arjun Thakur';  // var --> variable(key)/variable declaration    name --> variable Name   :   'Arjun Thakur'  -->  Value
```

***Naming Convention in javascript***
* *The first character must be a letter or an underscore `(_)` or an dollar `($)`. You cam't use a number as the first character.*
* *The rest of the variable name can inculde any letter, any Number, or the underscore. Can't use any other characters, inculding spaces.*
* *Variable names are case sensitive.*
* *No limit to the length of the variable name.*
* *You can't use one of the javaScript's reserved words as a variable name.*

## ***Q7. Data types in Javascript.***

*Every Variable has a data type that tells what kind of data is being stored in a variable. There are two types of data types in JavaScript namely Primitive data types and Non-primitive data types.*

***Primitive data types:*** *The predefined data types provided by JavaScript language are known as primitive data types. Primitive data types are also known as in-built data types.*

***Non-primitive data types:*** *The data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types. It is also known as derived data types or reference data types.*

***Primitive vs Non-Primitive***
| Primitive                              | Non-Primitive                                |
|   :---------: | :---------: |
| Primitive Data types are predefined | Non-Primitive data types are created by programmer|
| Primitive Data types will have certain values  | Non-Primitive data types can be NULL|
|Size depends on type on data structure|Size are not fixed|
|Examples are numbers, string|Example are Array, Linked List|
|It can start with lowercase|It can start with uppercase|

***Seven Data types that are primitives***
* ****Undefined*** : typeof instance==="undefined"*
`Undefined is a primitive value automatically assigned to variables that have just been declared, or to formal arguments for which there are no actual arguments.`
* ****Boolean*** : typeof instance==="boolean"*
`In computer science, a Boolean is a logical data type that can have only the values true or false.`
* ****Number*** : typeof instance==="number"*
`Number for numbers of any kind: integer or floating-point, integers are limited by ±(253-1)..`
* ****String*** : typeof instance==="string"*
`A string is a sequence of characters used to represent text.`
* ****Bigint*** : typeof instance==="bigint"*
`BigInt is a numeric data type that can represent integers in the arbitrary precision format.`
* ****Symbol*** : typeof instance==="symbol"*
`Symbol is a primitive type for unique identifiers.`
`Symbols are created with Symbol() call with an optional description (name).`
`Symbols are always different values, even if they have the same name. If we want same-named symbols to be equal, then we should use the global registry: Symbol.`
* ****Null*** : typeof instance==="null"*
`A null value represents a reference that points, generally intentionally, to a nonexistent or invalid object or address.`
`In JavaScript, null is marked as one of the primitive values, because its behavior is seemingly primitive. However, when using the typeof operator, it returns "object".`

## ***Q8. What is NaN?***
*The global `NaN` property is a value representing `Not-A-Number`.*
```javascript
    console.log('number'-'num')             //try this code
```
***Use of NaN***
```javascript
    var num = 12300;
    var name = "Arjun";
    console.log(isNaN(num));    //false
    console.log(isNaN(name));   //true
```
## ***Q9. Operators & Expressions ?***
*Expressions perform specific actions, based on an operator, with one or two operands. An operand can be a constant, a variable or a function result. Operators are arithmetic, logical, and relational. As with C, some operators vary in functionality according to the data type of the operands specified in the expression.*

* *Arithmetic operators*
    - *Unary operators*
    - *Binary operators*
* *Assignment operators*
* *Comparison operators*
* *Logical operators*
* *String operators*
* *Conditional (ternary) operator*

***Other operators***
* *Bitwise operators*
* *BigInt operators*
* *Comma operator*
* *Relational operators*

### ***Arithmetic operators ( +, -, * , ** , /, % )***
*Arithmetic operators perform mathematical operations such as addition and subtraction with operands. There are two types of mathematical operators: unary and binary. Unary operators perform an action with a single operand. Binary operators perform actions with two operands. In a complex expression, (two or more operands) the order of evaluation depends on precedence rules.*
***Unary arithmetic operators***
*Unary operators are arithmetic operators that perform an action on a single operand.*

___Increment operator & Decrement operator___

```javascript
    A=1; 
    B = A++; // b will equal 1, a will equal 2;  Increment operator (value 1st / inc. 2nd)
    A = 1; 
    B = ++A; // b will equal 2, a will equal 2; Increment operator (inc. 1st / value 2nd
    A= 1; 
    B = A--; // b will equal 1, a will equal 0; Decrement operator (value 1st / dec. 2nd
    A= 1; 
    B = --A; // b will equal 0, a will equal 0; Decrement operator  (dec. 1st / value 2nd
```
***Binary arithmetic operators***
*Insert a space before and after an arithmetic operator.*

|Symbol|Operation|Example|Description|
| :--: | :-----: | :---: | :------- |
|+|Addition|a + b|Add the two operands|
|-|Subtraction|a - b|Subtract the second operand from the first operand|
|*|Multiplication|a * b|Multiply the two operands|
|/|Division|a / b|Divide the first operand by the second operand|
|**|Power|a ** b|Raise the first operand by the power of the second operand|
|%|Modulo|a % b|Divide the first operand by the second operand and yield the remainder portion|

***Operator precedence***
*`Expressions are normally evaluated left to right.` Complex expressions are evaluated one at a time. The order in which the expressions are evaluated is determined by the precedence of the operators used. The standard C ordering is followed*
* *negation (-) unary*
* *power*
* *multiplication, division and modulo*
* *addition and subtraction*
>  If an expression contains two or more operators with the same precedence, the operator to the left is evaluated first. For example, 10 / 2 * 5 will be evaluated as (10 / 2) and the result multiplied by 5.

>When a lower precedence operation should be processed first, it should be enclosed within parentheses. For example, 30 / 2 + 8. This is normally evaluated as 30 divided by 2 then 8 added to the result. If you want to divide by 2 + 8, it should be written as 30 / (2 + 8).

>Parentheses can be nested within expressions. Innermost parenthetical expressions are evaluated first.

### ***Assignment operators***
*An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand.*

***There are also compound assignment operators***
|Name   |Shorthand operator|Meaning|
| :------   |:------:   |:------:  |
|Assignment|`x = f()`|`x = f()`|
|Addition assignment|`x += f()`|`x = x + f()`|
|Subtraction assignment|`x -= f()`|`x = x - f()`|
|Multiplication assignment|`x *= f()`|`x = x * f()`|
|Division assignment|`x /= f()`|`x = x / f()`|
|Remainder assignment|`x %= f()`|`x = x % f()`|
|Exponentiation assignment|`x **= f()`|`x = x ** f()`|
|Left shift assignment|`x <<= f()`|`x = x << f()`|
|Right shift assignment|`x >>= f()`|`x = x >> f()`|
|Unsigned right shift assignment|`x >>>= f()`|`x = x >>> f()`|
|Bitwise AND assignment|`x &= f()`|`x = x & f()`|
|Bitwise XOR assignment|`x ^= f()`|`x = x ^ f()`|
|Bitwise OR assignment|`x |= f()`|`x = x | f()`|
|Logical AND assignment|`x &&= f()`|`x && (x = f())`|
|Logical OR assignment|`x ||= f()`| `x || (x = f())`|
|Nullish coalescing assignment|`x ??= f()`|`x ?? (x = f())`|

### ***Comparison operators***
*A comparison operator compares its operands and returns a logical value based on whether the comparison is true.*

|Operator|Description|Examples returning true|
|--------|-----------|-----------------------|
|Equal (==)|Returns true if the operands are equal.|`3 == var1` `"3" == var1` `3 == '3'`|
|Not equal (!=)|Returns true if the operands are not equal.|`var1 != 4` `var2 != "3"`|
|Strict equal (===)|Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS.|`3 === var1`|
|Strict not equal (!==)|Returns true if the operands are of the same type but not equal, or are of different type.|`var1 !== "3"`  `3 !== '3'`|
|Greater than (>)|Returns true if the left operand is greater than the right operand.|`var2 > var1` `"12" > 2`|
|Greater than or equal (>=)|Returns true if the left operand is greater than or equal to the right operand.|`var2 >= var1`  `var1 >= 3`|
|Less than (<)|Returns true if the left operand is less than the right operand.|`var1 < var2` `"2" < 12`|
|Less than or equal (<=)|Returns true if the left operand is less than or equal to the right operand.|`var1 <= var2`    `var2 <= 5`|

>Note: `=>` is not a comparison operator but rather is the notation for Arrow functions.

### ***Bitwise operators***
*A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers.*

|Operator|Usage|Description|
|:------:|:---:|:---------|
|Bitwise AND|`a & b`|Returns a one in each bit position for which the corresponding bits of both operands are ones.|
|Bitwise OR|`a | b`|Returns a zero in each bit position for which the corresponding bits of both operands are zeros.|
|Bitwise XOR|`a ^ b`|Returns a zero in each bit position for which the corresponding bits are the same. [Returns a one in each bit position for which the corresponding bits are different.]|
|Bitwise NOT|`~ a`|Inverts the bits of its operand.|
|Left shift|`a << b`|Shifts a in binary representation b bits to the left, shifting in zeros from the right.|
|Sign-propagating right shift|`a >> b`|Shifts a in binary representation b bits to the right, discarding bits shifted off.|
|Zero-fill right shift|`a >>> b`|Shifts a in binary representation b bits to the right, discarding bits shifted off, and shifting in zeros from the left.|

***Example***

|Expression|Result|Binary Description|
|:--------:| :--: | :---------------: |
|`15 & 9`|9|`1111 & 1001 = 1001`|
|`15 | 9`|15|`1111 | 1001 = 1111`|
|`15 ^ 9`|6|`1111 ^ 1001 = 0110`|
|`~15`|-16|`~ 0000 0000 … 0000 1111 = 1111 1111 … 1111 0000`|
|`~9`|-10|`~ 0000 0000 … 0000 1001 = 1111 1111 … 1111 0110`|

### ***Logical operators***
*Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the **`&&`** and **`||`** operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value.*

***The logical operators are described in the following table.***
|Operator|Usage|Description|
|:------:|:---:|:----------|
|Logical AND (`&&`)|`expr1 && expr2`|Returns `expr1` if it can be converted to `false`; otherwise, returns `expr2`. Thus, when used with Boolean values, `&&` returns `true` if both operands are true; otherwise, returns `false`.|
|Logical OR (`||`)|`expr1 || expr2`|Returns `expr1` if it can be converted to `true`; otherwise, returns `expr2`. Thus, when used with Boolean values, `||` returns `true` if either operand is `true`; if both are false, returns `false`.|
|Logical NOT (`!`)|`!expr`|Returns `false` if its single operand that can be converted to `true`; otherwise, returns `true`.

***Examples of the && (logical AND) operator.***
```javascript
const a1 =  true && true; // t && t returns true
const a2 =  true && false; // t && f returns false
const a3 = false && true; // f && t returns false
const a4 = false && (3 === 4); // f && f returns false
const a5 = 'Cat' && 'Dog'; // t && t returns Dog
const a6 = false && 'Cat'; // f && t returns false
const a7 = 'Cat' && false; // t && f returns false
```

***Examples of the || (logical OR) operator.***
```javascript
const o1 =  true || true; // t || t returns true
const o2 = false || true; // f || t returns true
const o3 =  true || false; // t || f returns true
const o4 = false || (3 === 4); // f || f returns false
const o5 = 'Cat' || 'Dog'; // t || t returns Cat
const o6 = false || 'Cat'; // f || t returns Cat
const o7 = 'Cat' || false; // t || f returns Cat
```

***Examples of the ! (logical NOT) operator.***
```javascript
const n1 = !true; // !t returns false
const n2 = !false; // !f returns true
const n3 = !'Cat'; // !t returns false
```

### ***String operators***
*In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.*
```javascript
console.log('my ' + 'string'); // console logs the string "my string".
```
```javascript
let mystring = 'alpha';
mystring += 'bet'; // evaluates to "alphabet" and assigns this value to mystring.
```

### ***Conditional (ternary) operator***
*The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition.*
>The syntax is:- (condition ? val1 : val2)

*If condition is true, the operator has the value of val1. Otherwise it has the value of val2. You can use the conditional operator anywhere you would use a standard operator.*
```javascript
const status = age >= 18 ? 'adult' : 'minor';
```

### *Q10. What is = / == / === in JavaScript?*
* *`=`:-  `=` is simple assignment operator.*
* *`==`:- Returns `true` if operands have the same data type and same value, returns `false` if the values differ and also known as loose equality.Follows abstract equality comparison algorithm.*
* *`===`:- The `===` operators follow Strictly equality comparison algorithm, i.e., it doesn't do the type conversion of the operands before comparing their values and returns false even if the data type of the operands aren't the same.*

### *Q11. What is if / else if / else Statement and why we use it?*
*The `if...else` statement executes a statement if a specified condition is truthy. If the condition is falsy, another statement in the optional `else` clause will be executed.*

```javascript
if (condition)
  statement1

// With an else clause
if (condition)
  statement1
else
  statement2
```
***condition***
*An expression that is considered to be either truthy or falsy.*

***statement1***
*Statement that is executed if condition is truthy. Can be any statement, including further nested if statements. To execute multiple statements, use a block statement ({ /* ... */ }) to group those statements. To execute no statements, use an empty statement.*

***statement2***
*Statement that is executed if condition is falsy and the else clause exists. Can be any statement, including block statements and further nested if statements.*

***Note:- There is no elseif syntax in JavaScript. However, you can write it with a space between else and if. Multiple if...else statements can be nested to create an else if clause***

*You can combine as many logic operations as you want into one if statement using any of the javascript logic and comparision operators.*

### *Q12. What is Switch Statement in JavaScript?*
*The switch statement evaluates an expression, matching the expression's value against a series of case clauses, and executes statements after the first case clause with a matching value, until a break statement is encountered. The default clause of a switch statement will be jumped to if no case matches the expression's value.*

```javascript
const expr = 'Papayas';
switch (expr) {
  case 'Oranges':
    console.log('Oranges are $0.59 a pound.');
    break;
  case 'Mangoes':
  case 'Papayas':
    console.log('Mangoes and papayas are $2.79 a pound.');
    // expected output: "Mangoes and papayas are $2.79 a pound."
    break;
  default:
    console.log(`Sorry, we are out of ${expr}.`);
}
```

### *Q13. What is Loops & their types?*
*Loops are handy, if you want to run the same code over and over again, each time with a different value.*
***Instead of writing:***
```javascript
text += cars[0] + "<br>";
text += cars[1] + "<br>";
text += cars[2] + "<br>";
text += cars[3] + "<br>";
text += cars[4] + "<br>";
text += cars[5] + "<br>";
```
***You can write:***
```javascript
for (let i = 0; i < cars.length; i++) {
  text += cars[i] + "<br>";
}
```
### ***Different Kinds of Loops***
* *`for` - loops through a block of code a number of times*
* *`for/in` - loops through the properties of an object*
* *`for/of` - loops through the values of an iterable object*
* *`while` - loops through a block of code while a specified condition is true*
* *`do/while` - also loops through a block of code while a specified condition is true*

### ***For Loop***
*The for statement creates a loop with 3 optional expressions:* 
```javascript
for (expression 1; expression 2; expression 3) {
  // code block to be executed
}
or
for(initializer;condition;iteration){
  // code block to be executed
}
```
****Expression 1*** is executed (one time) before the execution of the code block.*

****Expression 2*** defines the condition for executing the code block.*

***Expression 3*** is executed (every time) after the code block has been executed.*

### ***While Loop***
*The `while` statement creates a loop that executes a specified statement as long as the test condition evaluates to true.*
***Syntax***
```javascript
while (condition)
  statement
```
***Example***
```javascrip
let n = 0;                    // Value declaration

while (n < 3) {             //  (n < 3 ) -> condition
  console.log("hello")
  n++;                     //   (n++) -> Statement
}

console.log(n);
```
### ***do...while***
*The `do...while` statement creates a loop that executes a specified statement until the test condition evaluates to false. The condition is evaluated after executing the statement, resulting in the specified statement executing at least once.*
***Syntax***
```javascript
do
  statement
while (condition)

```
***Example***
```javascrip
let result = '';
let i = 0;

do {
  i = i + 1;
  result = result + i;
} while (i > 5);

console.log(result);
// expected result: "1"
```
***Check Difference*** in upper code & bottom code
```javascrip
let result = '';
let i = 0;

do {
  i = i + 1;
  result = result + i;
} while (i < 5);

console.log(result);
// expected result: "12345"
```

### *Q14. What is function?*
*A JavaScript function is a block of code designed to perform a particular task.*
*A function is a group of reusable code which can be called anywhere in your program. This eliminates the need of writing the same code again and again.*

***function Definition***
*Before we use a function, we need to define it.*
*A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:*
* *The name of the function.*
* *A list of parameters to the function, enclosed in parentheses and separated by commas.*
* *The JavaScript statements that define the function, enclosed in curly brackets, {...}.*
```javascript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

***Calling functions***
* *Defining a function does not execute it.*
* *A JavaScript function is executed when "something" invokes it (calls it).*

***Function Parameter***
*Function parameters are the names listed in the function's definition.*

***Function Arguments***
*Function arguments are the real values passed to the function.*

***Function expressions***
*" Function expressions simply means create a function and put it into the variable "*

***Return Keyword***
*When JavaScript reaches a return statement, the function will stop executing.*
*Functions often compute a return value. The return value is "returned" back to the "caller".*

***Anonymous Function***
*A function expression is similar to and has the same syntax as a function declaration One can define "named" function expressions (where the name of the expression  might be used in the call stack for example) or "anonymous" function expressions.*

```javascript
function func(a=7,b=9){   //(a,b)->Function Parameter
  let sum=a+b;
  return sum;      //return sum value to our function 
}
console.log(func(3,6));     //(3,6)->Function Arguments
console.log(func());  //func()->Function call value already defined in function.
let value=func(2,10);   // Function expressions
console.log(value)

//Anonymous Function
const sum=function(a,b){
  return a+b;
}
console.log(sum(3,10))
```

