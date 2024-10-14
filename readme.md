# Run Github Google Apps Script in Google Apps

The purpose of this is to be able to maintain your Google Apps Scripts in a remote repo and edit them locally in a code editor.

This makes it easier to update, share and maintain Google Apps Scripts by keeping them in Github. 

This works with public or private repos because we use a [Github Token](https://github.com/settings/tokens) to pull the repo. 

## How to setup

The main file [github-sync.gs](github-sync.gs) has insturctions on how to customize the file. 

The main edits will be

### Notes

The script assumes you are using `http://www.mediawiki.org/xml/export-0.11/'  # Example namespace; adjust after printing structure` but it's possible your XML is using a different namespace. 

The script prints out the namespace when running and will throw an error if the namespace is incorrect but in the print it should indicate the correct namespace so you can update the namespace in Line 20 [max-word-count.py](max-word-count.py#L20) or [one-pdf.py](one-pdf.py#L20).

[^1]: The XML was generated utilizing [wikiteam3](https://github.com/mediawiki-client-tools/mediawiki-dump-generator)