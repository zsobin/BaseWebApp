# DemoWebApp

Check it out at: https://ancient-forest-87393.herokuapp.com/

Before starting:
- [ ] Create Heroku account (primary language = node) - https://signup.heroku.com/
  - [ ] download and install command line tools - https://toolbelt.heroku.com/
- [ ] Create Github account - https://github.com/join
  - [ ] download and install command line tools - https://help.github.com/articles/set-up-git/#setting-up-git
- [ ] download and install Node.js - https://nodejs.org/en/download/
- [ ] download and install a text editor (I recommend submlime text- https://www.sublimetext.com/3)

To set up and run:

1. Make a copy of my existing project on github
  - Fork the project at https://github.com/zsobin/DemoWebApp.git

2. Bring your new copy onto your computer from github 
  - `cd ~/Desktop`
  - `git clone https://github.com/YourUserName/DemoWebApp.git`
  - `cd DemoWebApp`
  - `ls`

3. Initialize it as a heroku project
  - `heroku login`
  - `heroku create`

4. Send the heroku project to heroku’s servers and view it online
  - `git push heroku master`
  - `heroku open`

5. Install the project’s dependencies and run the project on your local servers
  - `npm install`
  - `heroku local web`
  - check out http://localhost:5000
