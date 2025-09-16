## Setup

1. Install Poetry if you haven't already:
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

4. Change to python 3.12 and Activate the virtual environment:
```bash
poetry env use 3.12
source $(poetry env info --path)/bin/activate
```
5. Run adk
```
adk web
```
