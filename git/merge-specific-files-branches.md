# Merge Specific Files Between Branches

## Introduction
Git allows for the selective merging of files between branches, enabling developers to apply changes to only specific files rather than an entire branch.

## Steps

1. **Switch to the Target Branch**

    ``` 
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
