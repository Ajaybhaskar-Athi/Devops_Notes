The `git fetch` command is used to download commits, files, and references from a remote repository to your local repository without merging them into your local work. It updates your local copy of the remote branches but doesn't change your working directory.

Here’s what it does:

- Retrieves new changes (commits, branches, etc.) from the remote repository.
- Does **not** modify your working directory or current branch.
- Allows you to review the fetched changes before integrating them.

To integrate the changes into your current branch, you can use `git merge` or `git rebase` after fetching.

# .git/objects Created After Fetching

- As new data is fetched from the remote repository, Git creates new objects (blobs, trees, commits) in the local .git/objects directory.
- ` Each object is identified by a unique SHA-1 hash, which ensures that the data is consistent and integrity is maintained`
- After fetching, the new objects are stored in .git/objects, but your local references (like branches) are not updated immediately. Instead, they are updated in the refs directory (e.g., .git/refs/remotes/origin/) to track the state of the remote branches.

# STEPS:

1. git init
2. git remote add origin repo url # Add repo so in future its easy to pull or merge the fetched data
3. git fetch origin
4. git branch -r # list the branhces present in that fetched repo
5. cd .git/objects # navigate to local .git/objects directory where ur fethced data was there
6. ls # it lists the files avail in the .git/objects dir

` $ ls`
0a/ 17/ 24/ 32/ 43/ 46/ 57/ 76/ 85/ 91/ 98/ 9f/ ad/ d0/ e6/ f6/ pack/
0e/ 21/ 2e/ 35/ 45/ 54/ 5e/ 80/ 8d/ 96/ 9d/ ac/ c8/ dc/ ed/ info/ `
 `To know the SHA codes of the files navigate to that file using cd and run ls `

7. cd 0a
8. ls
   32c6b100a5d31e4635625f79798feOe7e687cf - some random code it will give this is the SHA-1 code of that

9. Git cat-file -t <sha-1 code of blob> # it will give the type of object
   `to run this command u make sure u r in 0a (whatever file) `
   ` And Add fileName+SHA code in above command => git cat-file -t 0a32c6b100a5d31e4635625f79798feOe7e687cf`

### Possible Outputs:

When you run the command, it will return the type of the object, which could be one of the following:

- **`blob`**: Represents file data (the content of a file).
- **`tree`**: Represents a directory structure and contains references to blobs and other trees.
- **`commit`**: Represents a commit in the repository, including metadata like author, timestamp, and a pointer to the tree object.
- **`tag`**: Represents an annotated tag that points to a commit.

### Example Usage:

If you have a SHA-1 hash like `a1b2c3d4e5f6g7h8i9j0`, you would run:

```bash
git cat-file -t a1b2c3d4e5f6g7h8i9j0
```

### Example Output:

If the SHA-1 corresponds to a blob object, the output would be:

```
blob
```

If it corresponds to a commit, the output would be:

```
commit
```

# In Git, a blob (short for "binary large object") refers to a specific type of object that represents the contents of a file. Here are the key points about blobs:

- Git cat-file -p <sha-1 code of blob> # it will give the contents of object
