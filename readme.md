## Setup

0. Setup your python venv -
```bash
conda create -n "myenv" python=3.12 ipython
```

1. Install Poetry - 
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

2. Install project dependencies:
```bash
poetry install
pip install google-adk
```

3. Set up gcloud and auth (better off doing this in a separate folder)
 ```bash
curl -o google-cloud-cli-darwin-x86_64.tar.gz https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-cli-darwin-x86_64.tar.gz
tar -xzf google-cloud-cli-darwin-x86_64.tar.gz
./google-cloud-sdk/install.sh

gcloud auth application-default login
```

4. Run adk
```
adk web
```
