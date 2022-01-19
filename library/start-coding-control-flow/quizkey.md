1. What does the following comparison statement return?

`7 === "7";`

Answer: false


2.What does the following comparison statement return?

`7 == "7";`

Answer: true

3. Which if block would you use to translate the following:
```
1.If timeOfDay is before noon (12), print "good morning!".
2. Otherwise, print "good night!".
```

Answer: 
```
if (timeOfDay < noon) {
console.log("good morning!")
} else {
console.log("good night!")
}
```

4. What will be output to the console after the code runs?
```
let count = 0;

if(count){
  console.log('Counting')
}else if(count > 0){
  console.log('Counting down')
}else if(count === 0){
  console.log('Done counting')
}
```
Answer: Done counting

5. What will be output to the console after the code runs?

```
let total = 10;
let amount = "10";

if(total === amount){
  console.log('Same')
}else if(total == amount){
  console.log('Similar')
}else if(total = amount){
  console.log('This is incorrect. Remember a single equals sign is for assignment, not for comparisons.')
}
```
Answer: Similar

6. What will be output to the console after the code runs?

```
let total = 10;

if(total >= 10){
  console.log('one')
}

if(total >= 0 && total > 100){
  console.log(' two')
}

if(total >= 0 || total > 100){
  console.log(' three')
}
```
Answer: one three

7. What will be output to the console after the code runs?
```
let isConnected = true;
console.log(!isConnected)
```
Answer: false
