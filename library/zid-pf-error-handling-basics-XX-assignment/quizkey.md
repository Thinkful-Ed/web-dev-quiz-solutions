**Error handling basics: Assignment**

1.  Take a moment to read through the code below.

**Answer: A -** throw "latitude, longitude, and passcode are required!";

2.  Using the same code from above, assume that the locations variable is an empty object.

What will be the last line of code run in the createSecretLocation() function if the function is called as follows:

**Answer: C -**`locations[lat][lon] = passcode; inside the catch block.`

3. Using the same code from above, assume that the locations variable looks like so:

**Answer:  C -** `locations[lat][lon] = passcode; inside the catch block.` 

4. Using the same code from above, assume that the locations variable looks like so:

**Answer: B -** `locations[lat][lon] = passcode; inside the try block.`

5. Take a moment to read through the code below.

**Answer: D -** There will be no return value. Instead, it will throw an error.

6. Using the same code from above, what will be the return value of the goToSecretLocation() function if it is called like so:

**Answer: A -** "Welcome." 

7. Using the same code from above, what will be the return value of the goToSecretLocation() function if it is called like so:

**Answer: C -** "You look around and don't see a thing."

8. Using the same code from above, what will be the return value of the goToSecretLocation() function if it is called like so:

**Answer: B -** "Nothing to see here!"
