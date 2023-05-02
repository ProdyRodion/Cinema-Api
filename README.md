# Dockerizing DRF Cinema

Cinema service made with DFR for management.

## 💼 Installing using GIT
```
git clone https://github.com/ProdyRodion/Cinema-DRF-api.git
cd cinema-api
python -m venv venv

On Mac and Linux:
source venv/bin/activate

On Windows:
venv/Scripts/activate

pip install -r requirements.txt
```

# 📝 Then do following steps
```python
export DB_HOST=<your db hostname>
export DB_NAME=<your db name>
export DB_USER=<your db user>
export DB_PASSWORD=<your db password>
export SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

# 📈 Run with DOCKER
```python
# DOCKER should be already installed
docker-compose build
docker-compose up
```

# 🤟 To get access to work with api do next steps
```python
create user via /api/user/register/
get access token via /api/user/token/
```

# 📜 Some project Features
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions
