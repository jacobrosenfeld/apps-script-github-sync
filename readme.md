# Run Github Google Apps Script in Google Apps

The purpose of this is to be able to maintain your Google Apps Scripts in a remote repo and edit them locally in a code editor.

This makes it easier to update, share and maintain Google Apps Scripts by keeping them in Github. 

This works with public or private repos because we use a [Github Token](https://github.com/settings/tokens) to pull the repo. 

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M314FOFQ)

## How to setup

The main file [github-sync.gs](github-sync.gs) has insturctions on how to customize the file. 

The main edit to the script itself is [Line 51](github-sync.gs#51) where you need to insert the name of the remote script to run. 

Otherwise all other variables should be within the Apps Script Editor variables. 

You need to create the following variables;

`GITHUB_TOKEN` Your personal token

`GITHUB_USER` The username of the repo owner

`GITHUB_REPO` The repo name 

`GITHUB_FILE_PATH` The git local filepath to the remote script, usually remote_script.gs

The next two variables are used if the remote script has a separate API that requires an API url and key. 

`api_url`

`api_key`