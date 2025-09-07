# Linux Commands

| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| echo | output any text | echo "Hello World!" | Hello World! |
| whoami | Find out what user we're currently logged in as! |
| man | 
| su | Switching between users | 
| ssh | secure shell | ssh username@10.x.x.x | 

## Troubleshooting
ipconfig - Displays IP configuration information.
ping - Tests connections to other IP hosts.
netstat - Displays network connections.
tracert - Displays the route taken to the destination.
nslookup - Directly queries the name server for information on a destination domain.

## File Systems

| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| ls | listing |
| cd | change directory |
| cat | concatenate; print file contents |
| pwd | print working directory |
| find | find file names; wildcard(*) | find -name *.txt | ./folder1/passwords.txt ./Documents/todo.txt |
| grep | earch the entire contents of this file | grep "81.143.211.90" access.log |
| touch |	touch	Create file |
| mkdir |	make directory	Create a folder |
| cp |	copy	Copy a file or folder |
| scp | secure shell copy to/from remote location | sch source_file username@10.X.X.X:/home/folder/file.txt |
| mv |	move	Move a file or folder |
| rm |	remove	Remove a file or folder |
| file |	file	Determine the type of a file |
| nano | terminal text editor |
| VIM | terminal text editor |
| wget | download file from the internet | wget file_url |

## Operators
| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| & |	This operator allows you to run commands in the background of your terminal. |
| && | This operator allows you to combine multiple commands together in one line of your terminal. |
| > | This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere. | echo hey > welcome.txt && cat welcome.txt | hey |
| >> | This operator does the same function of the > operator but appends the output rather than replacing (meaning nothing is overwritten). | echo you >> welcome.txt && cat welcome.txt | hey you |


## Processes

| Command | Description | Example Input | Example Output |
|---------|-------------|---------------|----------------|
| ps aux | display all system processes |
| systemctl [option] | stop/start/enable/disable a process | systemctl [stop/start/enable/disable] |
| crontab -e | Crontabs automation |
