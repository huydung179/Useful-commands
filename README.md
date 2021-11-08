# Useful-commands

## SSH

Forward ports:
`ssh -NfL [loginID]@[remote server]:[server post]:localhost:[local port]`

## Screen

Display all running sessions:
`screen -ls`

Create a new session:
`screen -S session_name`

Re-attach to a session:
`screen -r session_name`

Detach a session:
`Ctrl+a d`

Close a session: 
`Ctrl+a X`

Delete a session:
`screen -X -S session_name quit`

## Jupyter notebook

Set token for a notebook
`jupyter notebook --NotebookApp.token=abcd`

## Docker

Docker build:
`docker build -f [path to Dockerfile] -t [docker image's name] [path to building files or additional material]`

Alias in ~/.bashrc:
`alias nvidia-run="nvidia-docker run --rm -it --gpus=all --user=$(id -u):$(id -g) -v /etc/passwd:/etc/passwd:ro -v /etc/group:/etc/group:ro --shm-size 2056m"`

Run a docker:
`docker-run -v [local path]:[container path] [docker image's name] (bash)`
