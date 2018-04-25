# Config Heroku
```bash
npm install -g heroku
heroku login
```
# Deploy

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