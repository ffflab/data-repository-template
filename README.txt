data list
===

# Discription
A repository that collects only dvc files.
Pull the data/datasets you need.

# Setup
git clone dvc-data-list
cd dvc-data-list
pip install -r requirements.txt

# Pull
dvc pull sample.dvc

# Push
dvc push sample.dvc

# Switch remote
icloud_dir="$HOME/Library/Mobile Documents/com~apple~CloudDocs/dvcdata"
dvc remote add -f -d icloud ${icloud_dir}
dvc remote add -f -d gs gs://dvcspace-e1aa9a35
