**JavaScript foundations: Destructuring & Rest**


1. Evaluate the following code. What will be logged?

```javascript
const product = {
  name: "Geometric Print Swim Shorts",
  colors: {
    pink: {
      priceInCents: 1499,
      availableSizes: ["XS", "S", "M", "XL"],
    },
    blue: {
      priceInCents: 999,
      availableSizes: ["M", "L", "XL"],
    },
  },
};

const { colors: { pink } } = product;
console.log(pink);
```

**Answer: C**
```javascript
{
  priceInCents: 1499,
  availableSizes: ["XS", "S", "M", "XL"],
}
```

2. Evaluate the following code. What will be logged?

```javascript
const product = {
  name: "Geometric Print Swim Shorts",
  colors: {
    pink: {
      priceInCents: 1499,
      availableSizes: ["XS", "S", "M", "XL"],
    },
    blue: {
      priceInCents: 999,
      availableSizes: ["M", "L", "XL"],
    },
  },
};

const { colors: { pink: { availableSizes } } } = product;
console.log(availableSizes);
```

**Answer: D**
`["XS", "S", "M", "XL"]`

3.Evaluate the following code. What will be logged?

```javascript
const product = {
  name: "Geometric Print Swim Shorts",
  colors: {
    pink: {
      priceInCents: 1499,
      availableSizes: ["XS", "S", "M", "XL"],
    },
    blue: {
      priceInCents: 999,
      availableSizes: ["M", "L", "XL"],
    },
  },
};

const { colors: { pink: { availableSizes: [ first ] } } } = product;
console.log(first);
```

**Answer: E**
`"XS"`

4.  Evaluate the following code. What will be logged?

```javascript
const product = {
  name: "Geometric Print Swim Shorts",
  colors: {
    pink: {
      priceInCents: 1499,
      availableSizes: ["XS", "S", "M", "XL"],
    },
    blue: {
      priceInCents: 999,
      availableSizes: ["M", "L", "XL"],
    },
  },
};

const { colors: { pink: { availableSizes: [ first, ...rest ] } } } = product;
console.log(rest);
```

**Answer: F**
`["S", "M", "XL"]`

5.  Evaluate the following code. What will be logged?

```javascript
const product = {
  name: "Geometric Print Swim Shorts",
  colors: {
    pink: {
      priceInCents: 1499,
      availableSizes: ["XS", "S", "M", "XL"],
    },
    blue: {
      priceInCents: 999,
      availableSizes: ["M", "L", "XL"],
    },
  },
};


function printColors ({ colors }) {
  const result = Object.keys(colors);
  console.log(result.join(" and "))
}

printColors(product);
```

**Answer: B**
`"pink and blue"`
