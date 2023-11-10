# GIT TRICKS

## Commit
1. Undo last commit : [source](https://stackoverflow.com/questions/927358/how-do-i-undo-the-most-recent-local-commits-in-git)
    ```
    git reset HEAD~
    ```

## Stash
1. Stash your changes with a comment 
    ```
    git stash save "my comment"
    ```
2. To show the changes you made in a particular stash

    ```
    gitk stash@{0}
    ```
3. Delete top stash 
    ```
    git stash drop 
    ```
4. Delete nth stash  
    ```
    git stash drop stash@{n}
    ```
5. Clear all stash
    ```
    git stash clear
    ```
6.

