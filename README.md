brew install flyctl

mkdir hello-flask

cd hello-flask
python3 -m venv .venv
source .venv/bin/activate
python -m pip install Flask
python -m pip install gunicorn

flyctl launch
flyctl deploy