# Node File Handler

A Node.js app that reads commands associated with creating, appending, deleting, and renaming files from a file and executes them.

This app was developed in one of my videos in my Node.js course, "Understanding File System."

The application watches a file named "command.txt" for changes, and every time a change happens, it will read the file's content and do what the user specified.

For instance, if a user writes "create a file text.txt" in the command.txt file and saves it, a file named file.txt will be created in the working directory. We could also specify absolute paths.

We have these available operations:

- creating a file
- deleting a file
- renaming a file
- appending to a file

And we should write the commands in the following formats in the command.txt file:

- create a file \<path>
- delete the file \<path>
- rename the file \<path> to \<new-path>
- add to the file \<path> this content: \<content>

Note that we can only have and execute one command in the command.txt file at a time.

To run the application, clone the repo and run the following:

```
node app.js
```

The app will only use the native fs module, and there's no need to install other packages.
