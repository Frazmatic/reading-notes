# Using Git

## Navigation

[Introduction](https://frazmatic.github.io/reading-notes/) | [Growth Mindset](https://frazmatic.github.io/reading-notes/growth-mindset) | [Learning Markdown](https://frazmatic.github.io/reading-notes/learning-markdown) | [Text Editors](https://frazmatic.github.io/reading-notes/text-editor) | [Using Git](https://frazmatic.github.io/reading-notes/using-git) | [Learning HTML](https://frazmatic.github.io/reading-notes/learning-html)

## Git

Version control is a system for recording, and revisiting, changes to a file (or set of files). A Version Control System is a system for managing version control. Git (named after the British slang term) is a distributed version control system. GitHub is service where people can store and share their repositories, sort of like Youtube for Git.

Git uses snapshots to track changes. Every time a change is committed, a snapshot is created. Each new snapshot is a new version of the file(s).

If a file has been changed but a snapshot has not been created (it has not been committed) then it is in a “modified state”.  When a modified file is added using the `git add [filename]` command, it is tracked and ready to be committed (staged). It can then be committed by using the `git commit [filename]` command. After committing, the file is in the “committed” state, stored safely in a snapshot. The repository can then be pushed to a remote repository using the `git push origin main` command (where origin is the server from which you cloned and main is your local branch).

The command `git clone [url]` can be used to copy a remote repository to your local machine, while `git remove -v` will show short names next to their corresponding URLs (e.g. origin next to the URL you cloned from).
