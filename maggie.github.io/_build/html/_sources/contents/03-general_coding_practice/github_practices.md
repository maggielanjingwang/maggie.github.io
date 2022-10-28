# Best Github Practices & Workflow

All developers should aim to follow the outlined steps below when making any changes to the source code.


1. Raise a new issue in the ['Issues' tab](https://github.com/xf4j/registry-database/issues) and title the issue with the appropriate label (see Github Issue Labels). 
    - Provide a description of the nature of the features/changes you are planning to make, if necessary.  <br>
    - Under the 'Assignees' section on the right column of the page, assign yourself to the issue.  <br>
    - Under the 'Development' section on the right column of the page, create a branch for the issue. By standard, the branch name should be `issue-##`.  
        > Example: If you are working on issue #72, then the branch name linked to the issue should be `issue-72`.  

2. In your local terminal, fetch and pull the branch from the remote repository. 
    ```
    git fetch origin issue-##
    git checkout issue-##
    ```
3. As you are working on the local branch, make sure to periodically pull changes from the `origin/main` branch to avoid any merge conflicts down the line. You may have to sort out any merge conflicts locally if you are making changes to a file that has also been changed in `main`. Make sure to also do this before pushing 
    ```
    git pull origin main
    ```

4. Once you have finished making changes, push your changes to the remote repository. 
    ```
    git push
    ```

5. On the repository Github page, create a pull request (PR). 
    - Provide a description of the changes you have made in the comments.
    - Under the 'Reviewers' section on the right column of the page, add `xf4j` and `xfeng-carina` as reviewers.

