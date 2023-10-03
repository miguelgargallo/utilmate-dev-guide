# Merging Specific Files from `dev` to `main`

## Steps

1. **Checkout the Target Branch**: Make sure you are in the branch where you want to apply the changes (in this case, `main`).

```bash
git checkout main
```

2. Optional **Pull**: If you want to make sure you have the latest changes from the remote repository, you can pull them now.

```bash
git pull origin main
```

3. **Cherry-Pick Specific Files**: Use the `git checkout` command followed by the source branch name (`dev` in your case) and the paths to the specific files you want to merge.

```bash
git checkout dev -- path/to/image.svelte path/to/language.svelte
```

4. **Commit and Push**: Now, commit these changes and push them to the remote repository.

```bash
git commit -m "Merged specific files from dev"
git push origin main
```

5. **Resumen**: 

```bash
git checkout main
git checkout dev -- path/to/image.svelte path/to/language.svelte
git commit -m "Merged specific files from dev"
git push origin main
```

## Glossary
- **Cherry-Pick**: The act of choosing specific changes from one branch and applying them onto another.
- **Commit**: A set of changes to a repository.
- **Push**: The act of updating the remote repository with local changes.

## Historical Context
The concept of "cherry-picking" changes in version control dates back well before Git. However, Git has made it particularly easy to apply this strategy, allowing developers great flexibility in managing branches.
