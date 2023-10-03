# Merge Specific Files Between Branches

## Introduction
Git allows for the selective merging of files between branches, enabling developers to apply changes to only specific files rather than an entire branch.

## Steps

1. **Switch to the Target Branch**

    ``` w
    git checkout main

    ```

2. **Fetch the Latest Changes (Optional)**

    ``` 
    git pull origin main

    ```

3. **Checkout Specific Files from Source Branch**

    ``` 
    git checkout dev -- path/to/image.svelte path/to/language.svelte

    ```

4. **Commit Changes**

    ``` 
    git commit -m "Merged specific files from dev to main"

    ```

5. **Push Changes to Remote Repository**

    ``` 
    git push origin main

    ```

## Conclusion
By following these steps, you can selectively merge files from one branch into another without affecting the rest of the branch.

# Vocabulary and Historical Context
Git: A distributed version control system, initially developed by Linus Torvalds in 2005. It's widely used for source code management.

Branch: In Git, a branch is essentially a unique set of code changes with a unique name. The main or master branch is usually the default and is often considered as the "final" version of the project.

Commit: A commit, or "revision", is an individual change to a file (or set of files). It's like when you save a file, except with Git, every time you save it creates a unique ID that allows you to keep record of what changes were made when and by who.

Checkout: The act of switching between different versions of a target repository. In this context, you are "checking out" specific files from the dev branch to bring them into the main branch.

Pull: Fetching the latest changes from an online repository without merging them is known as pulling. In the context of GitHub, this is done using git pull.

By understanding these terms and their historical context, you can better appreciate the functionalities that Git offers for code management and collaboration.