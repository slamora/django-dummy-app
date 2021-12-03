# django dummy app
How to deploy it


1. Install Python and its packet manager (pip) 
```bash
# on a Debian based environment:
apt=(
    git
    python3-pip
    python3-setuptools
)
sudo apt-get install --no-install-recommends -y ${apt[@]}

```

2. Clone this repository
```bash
git clone https://github.com/slamora/django-dummy-app.git django-dummy-app
```

3. Prepare env and install requirements
```bash
cd django-dummy-app
python3 -m venv env
source env/bin/activate
pip3 install -r requirements.txt
```

4. Start django devel server (check everything is ok)
```bash
python manage.py migrate
python manage.py runserver
```

6. Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

7. If everything works, follow [Django deployment instructions](https://docs.djangoproject.com/en/2.1/howto/deployment/).
