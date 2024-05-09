# What does mean new Date() in JavaScript?
## In JavaScript, date objects are created with new Date(), returns a date object with the current date and time. And is looks our computer time an returns it. And also it will start from the 1st of Jenuary in the year 1970.
![alt text](./Без%20названия.png)


## In JavaScript there is 4 ways to create a new Date()
### 1.new Date()
### 2.new Date(milliseconds)
### 3.new Date(data string)
### 4.new Date(year, month, day, hours,minutes,seconds,milliseconds)


## 1.new Date()
### If we write just new Date it will return our laptop time.
#### For Example:
```javascript
let date = new Date()
console.log(date)
// Expected Output: 2024-05-08T14:42:52.943Z
```


## 2.new Date(miliseconds)
### In this way we should write a number and it will get it like a miliseconds and if we log it it will add the year 1970 with our miliseconds.
#### For Example:
``` javascript
let date = new Date(1000000)
console.log(date)
// Expected Output: 1970-01-01T00:16:40.000Z
```

## 3.new Date(string)
### In this one we should write any data and it will return this data.
#### For Exapmle:
``` javascript
let date = new Date()
console.log(date)
// Expected Output: 2024-10-13T06:13:00.000Z
```

## 4.new Date(year,month,day, ...)
### In this way we should write the year, month, day, date, minut, seconds and miliseconds. And it will returns as the same in new Date(string).
#### For Example:
``` javascript
let date = new Date(2024, 7, 5, 33, 33, 0)
console.log(date)
// Expected Output: 2024-08-06T04:33:00.000Z
```

# And the important thing is that Data has methods!!!
## 1.The first one is methods get, it means these methods starts with get.
![alt text](./Без%20названия.jpg)

## 1.What is method getFullYear() in JavaScript?
### This methods returns the year of the Data.
![alt text](./Без%20названия%20(1).png)
#### For Example:
``` javascript
let data = new Date('7/05/2024')
console.log(data.getFullYear())
// Expected Output: 2024
```

## 2.What is methods getMonth() in JavaScript?
### This methods returns the month of the Data and it doesn't have any parametrs.
![alt text](./Без%20названия%20(2).png)
#### For Example:
``` javascript
let data = new Date('07/05/2024')
console.log(data.getMonth())
// Expected Output: 06
```
#### Hear it returned us 6 but not 7 why? because it will count from index 0, index will start from 0.

## 3.What is method getDate() in JavaScript?
### This method will return the Date of the Date.NOT Day!!!
![alt text](./Без%20названия%20(3).png)
#### For Example:
``` javascript
let data = new Date('07/05/2024')
console.log(data.getDate())
// Expected Output: 5
```

## 4.What is method getDay() in JavaScript?
### This method returns the Day of the Date.
![alt text](./Без%20названия%20(4).png)
``` javascript
let data = new Date('07/05/2024')
console.log(data.getDay())
// Expected Output: 5
```
### As you can see it returned the day of the date

## 5.What is method getHours() in JavaScript?
### This method returns the time of the Data.
![alt text](./Без%20названия%20(5).png)
``` javascript
let data = new Date('07/05/2024/15:00')
console.log(data.getHours())
// Expected Output: 15
```

## 6.What is method getMinutes() in JavaScript?
### This method returns the minutes of the Data.
![alt text](./Без%20названия%20(6).png)
``` javascript
let data = new Date('07/05/2024/15:59')
console.log(data.getMinutes())
// Expected Output: 59
```


## 7.What is method get getSeconds() in JavaSxript?
### This method returns the seconds of the Data.
![alt text](./Без%20названия%20(7).png)
``` javascript
let data = new Date('07/05/2024/15:59:45')
console.log(data.getSeconds())
// Expected Output: 45
```

## 8.What is method getMiliseconds() in JavaScript?
### This methods returns the miliseconds of the Data.
![alt text](./Без%20названия%20(8).png)
``` javascript
let data = new Date('07/05/2024/15:59:19')
console.log(data.getMilliSeconds())
// Expected Output: 19
```
## After every seconds it will change. Don't forget about this.


## 9.What is method getTime() in JavaScript?
## This method returns the number of milliseconds since January 1, 1970.
![alt text](./Без%20названия%20(9).png)
``` javascript
let data = new Date('07/05/2024')
console.log(data.getMilliSeconds())
// Expected Output: 1720119600000
```

## 10.What is method Data.now() in JavaScript?
### This method also works as same as getTime(), counts the number of miliseconds since Jenuary 1,1970, but Data.now() is the static method of the Data Object. It means that we cannot write with any name we want like myDate.now or anything else. The syntax of this method is always Data.now()
![alt text](./Без%20названия%20(10).png)
``` javascript
let miliseconds = Date.now()
console.log((miliseconds))
// Expected Output: 1715187417838
```

# 2.And also we have methods starting with set.These methods will just add any year, month, date, day, seconds, milliseconds and etc.

# 3.What is new Map() in JavaScript?
## Map is a collection of elements that is elements are stored as a key, value.
![alt text](./Без%20названия%20(11).png)
``` javascript
let arr = ([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
console.log(arr);
// Expected Output: [
//   [ 'name', 'Eshmat' ],
//   [ 'surname', 'Toshmat' ],
//   [ 'FullName', 'Eshmat Toshmatov' ]
// ]
```


## new map has methods foritself()
### 1.set()
### 2.get()
### 3.delete()
### 4.has()
### 5.forEach()
### 6.enteries()
### 7.size

## 1.Method set() will set a new key with value in our Map.
``` javascript
let arr = new Map([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
console.log(arr.set('name', 20));
// Expected Output: Map(4) {
//   'name' => 'Eshmat',
//   'surname' => 'Toshmat',
//   'FullName' => 'Eshmat Toshmatov',
//   'age' => 20
// }
```

## 2.In Method get() we should call the key of the value and it will retu the value
### For Example:
``` javascript
let arr = new Map([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
console.log(arr.get('name'));
// Expected Output: 'Eshmat'
```

## 3.Method delete() will delete any key and returns a boolean answer true or false.
### For Example:
``` javascript
let arr = new Map([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
console.log(arr.delete('name'));
// Expected Output: true
```
### It returned true it will delete that key and says that I deleted this key, it means true.

## 4.Method has() also returns boolean asnwer it searchs the key that we need.
### For Example:
``` javascript
let arr = new Map([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
console.log(arr.has('FullName'));
console.log(arr.has('age'))
// Expected Output: true
// Expected Output: false
```

## 5.Method forEach() works as a Loop.
``` javascript
let arr = new Map([
    ['name', 'Eshmat'],
    ['surname', 'Toshmat'],
    ['FullName', 'Eshmat Toshmatov'],
]);
return arr.forEach((el) => {
    console.log(el)
});
// Expected Output: Eshmat Toshmat Eshmat Toshmatov
```

## 6.Method enteries() returns an object as an array


## 7.Method size returns the number of elements in a Map
### For Example:
``` javascript
let arr = new Map([
    ['name', 'Muborakshoh'],
    ['surname', 'Qurbonzoda'],
    ['age', '10']
]);
console.log(arr.size);
// Expected Output: 3
```


# What is new Set in JavaScript?
## new Set is a collection of elements or items that are unique. Any elements or items cannot repeat. new Set is in EcmaScript 6. The new Set can care any type either Primtives or Objects.
``` javascript
let letters = new Set(["a","b","c"]);
console.log(letters);
// Expected Output: Set(3) { 'a', 'b', 'c' }
```
### It will return in an Object.

# And also new Set() have methods for itself.

## 1.What is method add() of new Set() in Javascript?
### add() is a method that adds any elements or items with value we want with any type.
![alt text](./Без%20названия%20(1).jpg)
### For Example:
``` javascript
let new = new Set('Hello')
console.log(new.add('John'))
// Expected Output: 'Hello John'
```

## 2.What is method delete() of new Set() in JavaScript?
### Method delete is a method that deletes any elements ot item we want.
![alt text](./Без%20названия%20(12).png)
``` javascript
let mySet = new Set(['A','B','C','D','E'])
mySet.delete('E')
console.log(mySet);
// Expected Output: Set(4) { 'A', 'B', 'C', 'D' };
```

## 3.What is method has() in Javascript?
### Method has is a method that searchs an element or an item we want and returns boolean answer true or false.
#### For Example:
``` javascript
let mySet = new Set(['A','B','C','D','E'])
console.log(mySet.has('D'));
console.log(mySet.has('F'));
// Expected Output: True
// Expected Output: False
```

## 4.What is method values() in Javscript?
### Method values() is a method that return the values of the new Set().
``` javascript
let mySet = new Set(['A','B','C','D','E'])
let val = mySet.values()
console.log(val);
// Expected Output: [Set Iterator] { 'A', 'B', 'C', 'D', 'E' }
```


## 5.What is method size() is Javascript?
### Method size() is a method that returns the number of the elements o items we can say.
#### For Example:
``` javascript
let mySet = new Set(['A','B','C','D','E'])
console.log(mySet.size);
// Expected Output: 5
```

# So, that was all about new Date(), new Map() and new Set(). Thanks for lisening.
![alt text](./Снимок%20экрана%202024-05-09%20110349.png)