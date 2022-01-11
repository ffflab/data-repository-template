data list
===

# Discription
A repository that collects only dvc files.
Pull the data/datasets you need.

# Setup
git clone dvc-data-list
cd dvc-data-list
dvc remote add -d -f icloud "$HOME/Library/Mobile Documents/com~apple~CloudDocs/dvcdata"

# Use
git pull thedata.dvc
