## Collaboration with GitHub: Assessment

1. Imagine you are working on a team with three other developers on the same repository. You've been tasked with building a new feature.

    What step should you take _first_ out of the following steps?

    **Answer:** D. Pull from the remote repository's main branch to your local main branch.

2. Imagine you are working on a team with three other developers on the same repository. You've been tasked with building a new feature and have completed your work on a feature branch in your local repository and have synced it with any new updates. 

    What's the _next step_ you should take?

    **Answer:** A. Push your feature branch to GitHub.

3. Imagine that you created a repository for a new project and you want to add collaborators so that they can contribute to your project.

    Which of the following will allow collaborators to contribute to your repository?

    **Answer:** C. Invite collaborators using the **Manage Access** setting of the repository.

4. Imagine you've been working on a personal feature branch called `new-team-form`. You've just completed your work and made a commit.

    Which of the following will correctly prepare your code to be pushed to GitHub, resolving conflicts?
    
    **Answer:** A. 

    ```
    git checkout main
    git pull origin main
    git checkout new-team-form
    git merge main
    git push origin new-team-form
    ```

5. In the following merge conflict, what does `HEAD` refer to?

    ```
    <<<<<<< HEAD
    function addTeam (teams, newTeam) {
    =======
    function addTeam (newTeam) {
    >>>>>>> main
        teams.push(newTeam);
    }
    ```

    **Answer:** A. Your current branch's last commit.
