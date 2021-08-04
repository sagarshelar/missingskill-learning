
# JavaScript

#### History : -
- JavaScript was craeted at Netscape by Brendan Eich in 1995. 
- Javascript one of the most important language for company.
- Javascript- originally named as Moche and later renamed as Livescript. 
- ECMA internatinal Organization standardised the language after its final submission.
- Javascript is just-in-time compiled high-level language.
- Javascript is also discriped as a core language of world wide web.
- Javascript is primarily used for backend.



#### Control Structure
- if else - Often used
- for - Abstraction
- switch case - Better ay available in javascript
- while - Normal use
- do while - Rarely use

#### Operators
- **Arithmetic operator**
    - **+** : - Addition 
    - **-** : - Subtraction 
    - **( * )** : - Mltiplication 
    - **/** : - Division
    - **%** : - Mod
- **Coparison Operator**
    - **==** : - Equal to
    - **===** : - Equal type or value
    - **!=** : - Not equal to
    - **>** : - Greater than
    - **<** : - Less than
- **Logical Operator**
    - **&&** : - Logical AND
    - **||** : - Logical OR 
    - **!** : - Logical NOT


- **Bitwise**
- **|, &, ~**
- **Ternary Operator**
- Ex.  : - **? : ((a+b === 1) ? c : d)**

#### Variables
- Javascript variables are dynamic in nature.
- Javascript variables are containers.
- Javascript decides variable type at runtime.
- There are two types of variables
    - **Primitive**
    - **Non-primitive**
- **Primitive**
    - string
    - number
    - boolean
    - undefined
    - Null
    - Symbol (ES6)


- **Non-Primitive**
    - Object {}
    ```js
    var obj = {
        key:"value"
    };
    ```

    - **Array []**
    ```js
    var arr = [2, 3, Null`, true, [], {}];
    ```
        
    - In javascript everything is an object.
    - In ES6 'const, let' are introduced.



-  Some Concatination Example which due to bug in addition ( + ) operator.
1. number + null : number Ex. 1 + null = 1
2. number + boolean : number Ex. 1 + true = 2
3. number + undefined : NaN Ex. 1 + undefined = NaN
4. number + string : string Ex. 1 + “11” = “111”
5. number + array : string Ex. 1 + [1,2,3] = “11,2,3”
6. number + object : string Ex. 1 + {} = “1[object,object]”
7. null + null : 0 Ex. null + null = 0
8. undefined + undefinded : NaN Ex. undefined + undefined = NaN
9. undefined + null : NaN Ex.undefined + null = NaN
10. Boolean + null : number Ex. true + null = 1
11. array + array : string Ex. [1,2,3] +[1,2,3] = “1,2,31,2,3”


- **falsy values =>** 
    - 0,null,NaN,""(empty string),undefined,
- **truthy values =>**
    - Other than this falsy values all are always truthy.


- Var This variable is declared in the ES5 script. It has functional scope. You can re-declare var many times. You can update the variable.

    ```js
    var VariableName = Value;
    var a = 10;
    var b = "myName";
    var c = "true";
    ```

- Let This variable is declared in ES6 due to the drawback of var Variable. It has lexical scope. You cannot redeclare let variable. You can update it.
    
    ```
    let VariableName = Value;
    let a = 5; 
    a = 7;
    let a =7; //will throw error
    ```


- const This variable is declared in ES6 due to the drawback of var Variable. It has lexical scope. You cannot redeclare const variable. You cannot update it.

    ```
    // Synatx: const VariableName = Value;
    const val= "Hi"; 
    val = "Welcome to JavaScript"; // throw error
    const val = "Hello";          //will throw error
    ```


#### **ES5**
- **var** : -
    - Can be reclared
    - Can be re-initialised
    - Functional scope
    - Get hoisted


#### **ES6**
- **let** : -
    - As per ES6 standards let cannot be redeclared
    - Can be re-initialised
    - Lexical scope
    - Does'nt get hoisted

- **const** : -
    - As per ES6 standards let cannot be redeclared
    - Cannot be re-initialised but non-primitive values can be updated.
    - Lexical scope
    - Does'nt get hoisted


### Function-
- If we want to reuse code then we use functions.
- A function is a block of code design to perform a specific task. 
- We can pass a function as parameter also.
- Pure Function doesn't modify values outside the function, Pure function also - returns the same values passed as input. 
- High order Function that takes a function as parameter and returns function.
    ```js
    // syntax-
    function add(a,b){	//defination of function
        retun a+b;		//prints o/p=77
    }
    add(23,54);	//calling function
    ```
- **function hoisting**
    - Function assignment dosen’t get hoisted only function declaration get hoisted.
    Ex.
    ```js
    user("name1");
    var user = function getUser(name){
    console.log(name);   // Prints : - Sagar
    };
    getuser("Sagar")
    ```
- **function acts like first class citizen**
    - hoisted
    - container
    - object
    - overrides.
    - scope- local and global
    - functions are acts like object
    - function can do anything in javascirpt, it has all priviledges.


#### IIFE

- IIFE stands for Immidiately Invoking Function Expression.
    - Function are executes once.
    - Self executing function.
    - If variable is declared inside iife and then the variable get destroyed affunction get closed.
    - Always use semicolon(;) before starting iife.
    - IIFE is always anonymous function.
    - Immidiate call after declaration.
    ```js
    // syntax-
    ;(function(par){
        var a=10;
        return a;
    })();
    ```
    
    
- **Higher Order Function**
    - Function is the first class citizen and function is also an Object .
    - In JavaScipt function can be assigned to a variable or passed as a variable.
    - Higher-Order function is a function that recieves as a parameter returns.
    - function returns function.
    ```js
    // syntax and example-
    const arr1 = [1, 2, 3];
    const arr2 = [];
    for(let i = 0; i < arr1.length; i++){
        arr2.push(arr1[i] * 2);
    }
    console.log(arr2); // prints [2, 4, 6]
    ```
- **Arrow Function**
    - anonymous function.
    - no need of function keyword.
    - no need of return keyword.
    ```js
    // simple Function Syntax
    simple function-
    function(a){
        returns a;
    }
    // arrow function-
    a => {a}
    ```
- **pure function** 
    - Pure function is a function in which when I pass the value it will always returns the same value(no modification).
    - It does not changes the input value.
    ```js
    synatx
    function add(a,b){
    return a+b;
    add(23,45);
    }
    ```


- **Inline function**
    - Function which is defined within a function call and accessible outside the call.
    - Inline function is also a higher order function.
    - In JavaScript inline function is Anonymous function which is assigned to a variable.
    - It is callback function.


#### Prototype in JavaScript.
    - JavaScript can also be stated as a prototype language.
    - prototype of an object is one type of object.
    - A prototype object  can be attached with properties and methods.
    - In Function prototype it uses to create a object of similar type. 
    - it is initialised with new keywords. Just like new object () or {}.
    - Using these keywords properties of prototype object can be refered
 
- **Built-in prototype in JavaScript**:
    - **Array Prototype** : -
        - Whenever .(dot) used in array.JS internally it converts into Array prototype which has all methods.
        - It holds several basic build in methods like
        - **unshift** : - adds element at first position.  
        - **shift** : - removes element at first position. 
        - **concat** : -  join two arrays.
        - **forEach** : -  For loop iteration. 
        - **map** : -  Transforming function / array.
        - **filter** : -  filter out deta from array itam
        - **includes** : - search for specific elemngt in array.
        - **join** : - join array elements using delimiter.
        - **push** :-  Add itam at end of array
        - **pop** : Remove itam from end of array
        - **sort***  : sort the array 
        - **slice** : slice the array.

Object prototype : -

- When dot (.) is used JavaScript Engine converts it into Object prototype which has
 make methods on which key can operated.


Function Prototype : -

To create a object of similar type.
- initialize using new keyword.
- properties are refered using this keyword.
