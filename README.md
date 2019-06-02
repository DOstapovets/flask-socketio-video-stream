Try it with:
```
virtualenv env --no-site-packages
source env/bin/activate
pip install -r requirements.txt
gunicorn --worker-class eventlet -b localhost:5500 livestream:app --reload\
```

Then, point to http://127.0.0.1:4000
