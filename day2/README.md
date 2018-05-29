## Notes on Day 2

### Shebang

- A pound---A sharp: #

  An exclamation point---A bang: !

  \#!---Shebang

- The path after the shebang will lead to an interpreter.

  `#!/bin/bash` determines that `/bin/bash` will execute the commands in the file.

- If no shebang is offered, the script will be executed using the current shell, which is not portable at all because you have no control on others' log-in shell when they execute your script.

### Shell built-in Command

- A shell built-in command does not need any external program to execute it.

- `echo` is a shell built-in command.
- use a shell built-in command `type` to tell whether a command is shell built-in or not.
- use `type -a <command name>` to find all the built-in command whose name is `<command name>` and display them in the order of executing.
- Use path to force shell to execute the command specified.
- The last item will make the script less portable

### Variable

- No need to specify the type
- No spaces around the equal sign