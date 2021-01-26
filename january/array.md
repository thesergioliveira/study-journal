# Classes Notes

## Working with arrays

### **<u>Declaring an array</U>**

> **`const arr1 = [];`** \
> **`const arr2 = ["Good", "Day"];`**\
> **`const arr3 = new Array();`** // This one, I have never seeing been used.\
> **`array.of(1, 2, 4); // [1, 2, 3]`**

### **<u>Methods</U>**

#### **Access, add or remove array elements:**

> 1- .Push;\
>  2- .splice\
>  3- .Pop; \
>  4- .Unshift;\
>  5- Math.ceil();

- <u>**Parse**</u>
  > 1- parse.Int();\
      2-  parse.Float();

> Note: There is also the possibility of using the "+str" and "str \* 1", in order to turn a string into a number. Those methods are **_not professional_**, thus the usage of it is to be discouraged.

````

 **<u>Typeof():</U>**
  > 1- let str1 = "4";\
          console.log(typeof str1); //string\
      2-  let x = 4;\
          console.log(typeof x); //number\
      3-  console.log(typeof console.log()); //function\
      4-  console.log(typeof Math); //object
<u>**Round:**</u>
  > 1- Up:\
          `function roundUp(num){
          let result = Math.ceil(num);
          console.log(result);
          }`\
      2-Down:\
          `function roundDown (num){
          let result = Math.floor(num);
          console.log(result);
          }`
- <u>**Math.randon: Random Number Generator**</U>
  > 1- Integers from 1-6(dice):\
          `console.log(math.floor(Math.random()* 6) +1);` //1 //4// //6 //3 //3...\
      2-  Float from 0-9:\
          `console.log(Math.random()*10);` //9.1234563456234578 //6.23454567412366547...


```diff
-  Note: Whenever wantinfg to return integers as a result of Math.random, use the function Math.floor to adjust the results of Math.random.
````

### <u>**Methods:**</u>

- <u>**toFixed**</u>
  > 1- `let floatFisrt = 34,,98834234\
          console.log(floatFisrt.toFixed(2));` // 34.98\
      2- `let num = 4\
          console.log(floatFirt.toFixed(num));` //3.9883

### <u>**Operators:**</u>

> - <u>**Increment and Decremnt**</u>
>   1- ++ ;\

    2- -- ;

> - <u>**Comparison**</u>
>   1- == ;\
>   2- !=;\
>   3- &&;\
>   4- ||;\
>   5- null has the value of false;\
>   6- 0 has the value of false;\
>   7- 1has the value of true;\
