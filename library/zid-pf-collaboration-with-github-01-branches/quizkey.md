**Collaboration with GitHub: Branches**

1. Which of the following would be a good name for a branch, according to the curriculum?

**Answer:  D** `az--new-feature`

2. Imagine the following two branches each have a number of commits:

```
master: A, B
feature-branch: A, B, X, Y
```

What would happen if the following command was run _from `feature-branch`_.

```bash
git merge feature-branch
```

**Answer:  A** You would receive an error, as you would be trying to merge `feature-branch` with itself.


3. Imagine the following two branches each have a number of commits:

```
master: A, B
feature-branch: A, B, X, Y
```

What would happen if the following command was run _from `master`_.

```bash
git merge feature-branch
```

**Answer:  D**  The `master` branch would now have commits "A", "B", "X", and "Y."
