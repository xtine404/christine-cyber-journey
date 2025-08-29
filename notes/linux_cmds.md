# Linux Commands

| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| echo | output any text | echo "Hello World!" | Hello World! |
| whoami | Find out what user we're currently logged in as! |

## File Systems

| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| ls | listing |
| cd | change directory |
| cat | concatenate; print file contents |
| pwd | print working directory |
| find | find file names; wildcard(*) | find -name *.txt | ./folder1/passwords.txt ./Documents/todo.txt |
| grep | earch the entire contents of this file | grep "81.143.211.90" access.log |

## Operators
| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| & |	This operator allows you to run commands in the background of your terminal. |
| && | This operator allows you to combine multiple commands together in one line of your terminal. |
| > | This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere. | echo hey > welcome.txt && cat welcome.txt | hey |
| >> | This operator does the same function of the > operator but appends the output rather than replacing (meaning nothing is overwritten). | echo you >> welcome.txt && cat welcome.txt | hey you |
