        JavaScript
       Assignment 6

Write short notes on Array methods with code example
1.push()
 
 -  The push() method adds new items to the end of an array. The push() method changes the length of the array
  ```js
                        let arr=[1,2,3,4,5]
                        let newArr=arr.push("six")
                        console.log(newArr);
```
2.pop()

 -  The pop() method removes (pops) the last element of an array. The pop() method changes the original array.
```js
                         let arr=[1,2,3,4,5]
                        console.log(arr.pop());
                        console.log(arr);
```

3.shift()

 -  The shift() method changes the original array. The shift() method returns the shifted element.
```js
                        let arr=[1,2,3,4,5]
                        console.log(arr.shift());
                        console.log(arr);
```
4.unshift()

  - The unshift() method adds new elements to the beginning of an array. The unshift() method overwrites the original array.
  ```js
                        let arr=[1,2,3,4,5]
                        console.log(arr.unshift("zero"));
                        console.log(arr);
```
5.includes()

  - The includes() method returns true if a string contains a specified string. Otherwise it returns false . The includes() method is case sensitive.
   ```js
                         let arr=[1,2,3,4,5]
                         console.log(arr.includes(3));
                         console.log(arr);
```
6.toString()

  -  The toString() method is used internally by JavaScript when an object needs to be displayed as a text (like in HTML)
   ```js
                        let arr=[1,2,3,4,5]
                        console.log(arr.toString());
                        console.log(arr);
```
7.reverse()

  -  The reverse() method reverses the order of the elements in an array. The reverse() method overwrites the original array.
   ```js
                      let arr=[1,2,3,4,5]
                      console.log(arr.reverse());
                      console.log(arr);
```
8.join()
   
  -  The join() method returns an array as a string. The join() method does not change the original array.
```js
                        let arr=[1,2,3,4,5]
                        console.log(arr.join());
                        console.log(arr.join(""));
                        console.log(arr.join(" "));
                        console.log(arr.join("-"));
                        console.log(arr.join("&"));
                        console.log(arr);
```
9.concat()

  -  The concat() method joins two or more strings. The concat() method does not change the existing strings. The concat() method returns a new string.
   ```js
   
                        let arr1=[1,2,3,4,5]
                        let arr2=[6,7]
                        let arr3=[8,9]
                        console.log(arr1.concat(arr2,arr3));
```
10.flat()

   - The flat() method of Array instances creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.
   ```js
                   let arr=[1,2,[3,4,5],[6,7],8]
                   console.log(arr.flat());
```
11.slice()

   - The slice() method returns selected elements in an array, as a new array. The slice() method selects from a given start 
   ```js
                 let arr=[1,2,3,4,5]
                 let newArr=arr.slice(0,1)
/                console.log(newArr)
```
12.splice()

   - The splice() method adds and/or removes array elements.The splice() method overwrites the original array.
```js
       let arr=[1,2,3,4,5]
       arr.splice(1,0,"one","two")
       console.log(arr)   
```      

    
  https://javascript-array-methods-quiz.netlify.app/



  ![ss](./WhatsApp%20Image%202024-09-30%20at%202.57.30%20PM.jpeg)


1.Write a JavaScript function to check whether an `input` is an array.
```js
function isArr(arr){
    return Array.isArray(arr)
}
console.log(isArr([1,2,3]))
```

2.Write a JavaScript function that takes an array as an argument and returns the first element of the array.

```js
                let firstElement=(arr)=>{
                return arr.slice(0,1)
                }
                console.log(firstElement([1,2,3]));

```
3.Write a JavaScript function that takes an array as an argument and returns the last element of the array.
```js
                let firstElement=(arr)=>{
                return arr.slice(2,3)
                }
                console.log(firstElement([1,2,3]));
```

4.Write a simple JavaScript function to join all elements of the following array into a string.
Sample array : myColor = ["Red", "Green", "White", "Black"];
```js
                let arr=["Red", "Green", "White", "Black"]
                console.log(arr.join(""))
```
5.Write a JavaScript program that accepts a number as input and inserts dashes (-) between each. For example, if you accept 025468 the output should be 0-2-5-4-6-8
```js
                let arr=[0,2,5,4,6,8]
                console.log(arr.join("-"));
```
6.Write a JavaScript function that checks if the given number is even or odd then returns a Boolean value (use: arrow function, return keyword, ternary operator)
```js
                let input=5
                let evenOrodd=(num)=>{
                let result=num%2===0?console.log("even"):console.log("odd");
                return result
                }
                evenOrodd(input)
```
7.Create an array of guestlist. Write a javascript function that takes the user’s name as an argument and checks whether it is in the guestlist. If yes, return the string “Welcome” else, return “Sorry, good luck next time”.

```js   
                
                let list=["sree","dev","gowtham","bipin","ayana","aswin"]
                let check=(name)=>{
                        if(list.includes(name)){
                                console.log("welcome");

                        }else{
                console.log("sorry");
         }
        }
        check("gowri")  
```

8.Write a javascript function that reverses a given number example: 123456789 => 987654321 (split(), reverse (), join())

```js
let num=123456789
let str=num.toString().split("").reverse().join("")
console.log(str);
```

9.Write a JavaScript function that accepts a string as a parameter and converts the first letter into upper case.
  Example: “javascript” => “Javascript”

```js
                let Name="javascript"
                let firstLetter=Name.slice(0,1).toUpperCase()
                let secondLetter=Name.slice(1,Name.length).toLowerCase()
                console.log(firstLetter+secondLetter)
  ```