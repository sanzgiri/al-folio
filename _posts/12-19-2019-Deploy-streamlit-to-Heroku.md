---
title: , 12-19-2019
date: 12-19-2019 00:00:00 Z
permalink: "Deploy-streamlit-to-Heroku-12-19-2019"
layout: post
excerpt: Deploy-streamlit-to-Heroku, 12-19-2019
---
### Deploy streamlit app to Heroku (on mac)
```
# Install heroku
brew install heroku/brew/heroku

# Setup autocomplete for heroku
heroku autocomplete

# Demo app
git clone https://github.com/MaartenGr/streamlit_guide.git
cd streamlit_guide/

# Deploy app
heroku login
heroku create
git push heroku master
heroku ps:scale web=1
heroku open
```
