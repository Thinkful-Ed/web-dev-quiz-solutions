Collaboration with GitHub: Assignment

1. Imagine you are working on a team with three other developers on the same repository. You've been tasked with building a new feature.

What step should you take _first_ out of the following steps?

**Answer:  D** Pull from the remote repository's master branch to your local master branch.

2. Imagine you are working on a team with three other developers on the same repository. You've been tasked with building a new feature and have completed your work on a feature branch in your local repository and have synced it with any new updates. 

What's the _next step_ you should take?

**Answer:  A** Push your feature branch to GitHub.

3. You're looking to add a feature to an existing repository. Unfortunately, while the repository is public, you do not have direct write access to the repository.

Which of the following is the correct process for adding a feature to the new repository.

**Answer: C** Fork and clone the repository. Then, add the new feature. Push your code to _your_ remote repository and then create a Pull Request, comparing your remote repository against the original remote repository.


4. Imagine you've been working on a personal feature branch called `new-team-form`. You've just completed your work and made a commit.
Which of the following will correctly prepare your code to be pushed to GitHub, resolving conflicts?

**Answer:  A** 

```
git checkout master
git pull origin master
git checkout new-team-form
git merge master
git push origin new-team-form
```

5. In the following merge conflict, what does `HEAD` refer to?

```js
<<<<<<< HEAD
function addTeam (teams, newTeam) {
=======
function addTeam (newTeam) {
>>>>>>> master
    teams.push(newTeam);
}
```

**Answer:  A** Your current branch's last commit.


