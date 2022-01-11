data list
===

# Discription
A repository that collects only dvc files.
Pull the data/datasets you need.

# Setup
git clone dvc-data-list
cd dvc-data-list

# Switch data remote
dvc remote add -f -d gs gs://dvcspace-e1aa9a35
dvc remote add -f -d icloud "$HOME/Library/Mobile Documents/com~apple~CloudDocs/dvcdata"

# Pull
dvc pull sample.dvc

# Push
dvc push sample.dvc