**Developer Workflow: File Paths**

1.
Imagine you are in the `mammal/` directory of the following file structure.

```
animal
├── mammal
│   ├── bovine
│   │   └── cow
│   ├── canine
│   └── equine
│       ├── horse
│       └── zebra
└── reptile
    ├── bird
    ├── lizard
    │   └── salamander
    └── snake
```

Which of the options is the correct path to the `cow/` directory?

**Answer:  C**
`./bovine/cow`

2.Imagine you are in the `reptile/` directory of the following file structure.

```
animal
├── mammal
│   ├── bovine
│   │   └── cow
│   ├── canine
│   └── equine
│       ├── horse
│       └── zebra
└── reptile
    ├── bird
    ├── lizard
    │   └── salamander
    └── snake
```

Which of the options is the correct path to the `canine/` directory?

**Answer:  C**
`../mammal/canine`

3.Imagine you are in the `mammal/` directory of the following file structure.

```
animal
├── mammal
│   ├── bovine
│   │   └── cow
│   ├── canine
│   └── equine
│       ├── horse
│       └── zebra
└── reptile
    ├── bird
    ├── lizard
    │   └── salamander
    └── snake
```

Which of the options is the correct path to the `zebra/` directory?

**Answer:  C**
`./equine/zebra`
