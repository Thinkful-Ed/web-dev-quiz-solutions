## Collaboration with GitHub: Merge requests

1. When does a merge conflict occur?

    **Answer:** B. When two commits from different branches edit the same line

2. Which of the following best describes the merge conflict below?

    ```
    <<<<<<< HEAD
    =======
    function playTrack(track) {
      const message = `Now playing ${track.name} by ${track.artist}`;
      console.log();
    }
    >>>>>>> main
    ```

    **Answer:** A. This conflict is a result of merging `main` into a feature branch. The code was deleted in the feature branch but was changed or added in the `main` branch.
