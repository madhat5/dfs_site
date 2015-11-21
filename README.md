---
---
DFS
---

- Members:
    - David
---

Links:

- Project:
    - GitHub
        - 
    - Heroku
        - 

- API's
    - http://espn.go.com/apis/devcenter/docs/
    - https://developer.yahoo.com/fantasysports/
    - http://developer.cbssports.com/documentation/api/files/sports
    - https://probasketballapi.com/docs/draftkings/players
    - http://armchairanalysis.com/data.php
    - http://www.fantasyfootballnerd.com/fantasy-football-api
    - http://www.rotowire.com/rss/
---
Technical Requirements:

---
Timeline goals:

Trello link: 

Wireframes: 

Git flow:

- Justin is Czar
- Steps:
    - git clone (SSH key)
    - Justin merges end of day
    - Team creates 1 branch per file task
        - from master
            - git checkout -b name_feature
    - Team pushes by end of day 
        - from branch
            - git add .
            - git commit -m "update details"
            - git push origin name_feature
        - slack note when pushed
    - Team pulls @ beginning of day
        - from master
            - git pull origin master

---
User story:

MVP:

- MOAR MODALS!!!

- landing page:
    - map
        - modal for location details
        - cannot add location until logged in
    - log in button
        - > opens user page
    - register buton
        - > opens register form

- user page
    - map
        - modal dislpays
            - task
            - location
            - details
            - button add to to-do
    - to do list (div)
        - task
        - button complete
            - complete pushes to Done
    - user updates button
        displays form 
        - edit
        - 
    - logout


+features:

- 




---
---
App Build Steps:

- touch server.js --x--

- npm init --x--
    - 'enter' through all the prompts

- express setup (npm install --save express) --o--
    - server.js
        - var express = require('express');
        - var app = express();

- set app port --o--
    - server.js
        - var port = process.env.PORT || 3000;

- morgan setup (npm install --save morgan) --x--
    - server.js
        - var morgan = require('morgan');
        - app.use(morgan('dev'));

- bodyparser setup (npm install --save body-parser) --x--
    - server.js
        - var bodyParser = require('body-parser');
        - app.use(bodyParser.urlencoded({ extended: false}));
        - app.use(bodyParser.json());

- mongoose setup (npm install --save mongoose) --x--
    - server.js
        - var mongoose = require('mongoose');
        - mongoose.connect('mongodb://localhost/db_name');

- md5 setup (npm install --save md5) --o--
    - server.js
        - var md5 = require('md5');

- cookies setup (npm install --save cookie-parser) --o--
    - server.js
        - var cookieParser = require('cookie-parser');
        - app.use(cookieParser());

- mkdir public --o--
    - server.js
        - app.use(express.static('public'));
    - touch public/index.html
    - touch public/app.js
    - touch public/style.css

- middleware setup --o--

- models --o--
    - mkdir models
        - touch models/user.js
        - touch models/task.js
    - server.js
        - var User = require('./models/user');
        - var Task = require('./models/task');

- test connection --o--
    - setup basic route
    - setup basic index.html/app.js
    - launch server (nodemon)

- >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>< HARD STOP ><<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

- CDN
    - Handlebars URL --x--
    - js-cookie URL --x--
        
- model build --o--
    - user.js
        - var mongoose = require('mongoose');
        - var userSchema = new mongoose.Schema({ ... });
            - link taskSchema
        - var User = mongoose.model('User', userSchema);
        - module.exports = User;
        - embed tasks (ref Complaints)
    - task.js
        - var mongoose = require('mongoose');
        - var taskSchema = new mongoose.Schema({ ... });
        - var Task = mongoose.model('Task', taskSchema);
        - module.exports = Task;
        - ?embed users?

- Story build --o--
    - server: 
        - server.js 
            - TEST 
    - client: --o--
        - TEST
        - index.html
        - app.js
            - user 
                - signup
                - update
                - delete
            - task
                - all
                - new
                - delete (auto delete when done)

- CSS --o--

- [seed 1 user + task --o--
    - node server.js]


---
---
Reference

- Git merging
    - https://github.com/ga-students/wdi_lettuce_students/blob/master/w08/d02/INSTRUCTOR/git_solo.md





---
---
Comments

- 






