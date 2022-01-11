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

# Add new data/dataset
git clone https://github.com/ffflab/data-repository-template
cd data-repository-template
wget -O lenna.png "https://upload.wikimedia.org/wikipedia/en/7/7d/Lenna_%28test_image%29.png"
dvc add lenna.png
dvc push
git add lenna.png.dvc
git commit -m "add lenna"
git push
