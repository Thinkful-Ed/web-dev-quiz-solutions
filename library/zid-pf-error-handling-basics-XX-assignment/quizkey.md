## Error-handling basics: Assessment

1.  Take a moment to read through the code below.

    ```js
    const locations = {};

    function createSecretLocation(lat, lon, passcode) {
      if (!lat || !lon || !passcode) {
        throw "latitude, longitude, and passcode are required!";
      }

      try {
        locations[lat][lon] = passcode;
      } catch (error) {
        locations[lat] = {};
        locations[lat][lon] = passcode;
      }
    }
    ```

    Assuming that the `locations` variable is an empty object, what will be the _last_ line of code run in the `createSecretLocation()` function if the function is called as follows:

    ```js
    createSecretLocation(40.35, -105.81);
    ```

    **Answer:** A. `throw "latitude, longitude, and passcode are required!";`

2.  Using the same code from above, assume that the `locations` variable is an empty object.

    What will be the _last_ line of code run in the `createSecretLocation()` function if the function is called as follows:

    ```js
    createSecretLocation(40.35, -105.81, "ROCKY-MOUNTAINS");
    ```

    **Answer:** C. `locations[lat][lon] = passcode;` inside the `catch` block.

3. Using the same code from above, assume that the locations variable looks like so:

    ```js
    const locations = {
      "40.35": {
        "-105.81": "ROCKY-MOUNTAINS"
      }
    }
    ```

    What will be the last line of code run in the `createSecretLocation()` function if the function is called as follows?

    ```js
    createSecretLocation(28.66, -105.81, "CHIHUAHUA-MEXICO");
    ```

    **Answer:** C. `locations[lat][lon] = passcode;` inside the `catch` block. 

4. Using the same code from above, assume that the `locations` variable looks like so:

    ```js
    const locations = {
      "40.35": {
        "-105.81": "ROCKY-MOUNTAINS"
      },
      "28.66": {
        "-105.81": "CHIHUAHUA-MEXICO"
      }
    }
    ```

    What will be the last line of code run in the `createSecretLocation()` function if the function is called as follows?

    ```js
    createSecretLocation(40.35, 22.54, "KATERINI-GREECE")
    ```

    **Answer:** B. `locations[lat][lon] = passcode;` inside the `try` block.

5. Take a moment to read through the code below.

    ```js
    const locations = {
      "40.35": {
        "-105.81": "ROCKY-MOUNTAINS",
        "22.54": "KATERINI-GREECE"
      },
      "28.66": {
        "-105.81": "CHIHUAHUA-MEXICO"
      }
    };

    function goToSecretLocation(lat, lon, passcode) {
      if (!lat || !lon || !passcode) {
        throw "latitude, longitude, and passcode are required!";
      }

      let result;
      try {
        if (locations[lat][lon] === passcode) {
          result = "Welcome.";
        } else {
          throw "Nothing to see here!";
        }
      } catch (error) {
        if (typeof error === "string") {
          result = error;
        } else {
          result = "You look around and don't see a thing.";
        }
      }

      return result;
    }
    ```

    What will be the return value of the `goToSecretLocation()` function if it is called like so?

    ```js
    goToSecretLocation(40.35, -105.81);
    ```

    **Answer:** D. There will be no return value. Instead, it will throw an error.
    
6. Using the same code from above, what will be the return value of the `goToSecretLocation()` function if it is called like so:

    ```js
    goToSecretLocation(40.35, 22.54, "KATERINI-GREECE");
    ```

    **Answer:** A. "Welcome." 

7. Using the same code from above, what will be the return value of the `goToSecretLocation()` function if it is called like so:

    ```js
    goToSecretLocation(65.99, 22.54, "ROCKY-MOUNTAINS");
    ```

    **Answer:** C. "You look around and don't see a thing."

8. Using the same code from above, what will be the return value of the `goToSecretLocation()` function if it is called like so:

    ```js
    goToSecretLocation(40.35, -105.81, "KATERINI-GREECE");
    ```

    **Answer:** B. "Nothing to see here!"
