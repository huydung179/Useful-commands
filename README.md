# Useful-commands

## Screen

Display all running sessions:
$ screen -ls

Create a new session:
$ screen -S session_name

Re-attach to a session:
$ screen -r session_name

Detach a session:
Ctrl+a d

Close a session: 
Ctrl+a X

Delete a session:
$ screen -X -S session_name quit

## Jupyter notebook

Set token for a notebook
$ jupyter notebook --NotebookApp.token=abcd
