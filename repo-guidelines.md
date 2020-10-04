# Guidelines

1. __Never__ commit and push any changes to upstream/master!

2. __Never__ change any of the `README.md` or other files in the repo, only add your own `solution` folder!

2. To get the latest changes from the upstream `codesy-students` repo (instructors version) run the following commands:
    1. `git fetch upstream`
    2. `git rebase upstream/master`

2. To commit and push your solution to each activity when you complete it:
    1. Choose the files you will commit for the solution and stage them using `git add <filename/folder>`. __NOTE:__ replace `<filename/folder>` with a file name or folder!
    2. Commit the staged files with `git commit -m "commit message goes here"`. __NOTE:__ write your own commit message, don't copy this one!
    3. Push your changes to your GitHub repo with `git push`.