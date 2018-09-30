# Config Heroku
```bash
npm install -g heroku
heroku login
```
# Set Environment Variable
```bash
heroku config:set NAME=<VALUE>
```

# Deploy App

```bash
git init
git add .
git commit -m "My first commit"
heroku create meu-app 
heroku buildpacks:set heroku/nodejs
heroku git:remote -a meu-app
git push heroku master
heroku ps:scale web=1
heroku logs --tail
heroku open
```
# Update App

```bash
git add .
git commit -m "My Second commit"
git push heroku master
heroku ps:scale web=1
heroku logs --tail
heroku open
```

# Heroku Clone
```bash
heroku git:clone -a myapp
```
