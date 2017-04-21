# Base Web App

Check it out at: https://pacific-bastion-31399.herokuapp.com/

### Phase 1: Hello World

Mission- Get up and running with the Base Web App. Should be able to run locally and be deployed on Heroku. 

##### 0. Before you get started:

- [ ] [Create Heroku account (primary language = node)](https://signup.heroku.com/)
- [ ] [Download and install Heroku's command line tools](https://toolbelt.heroku.com/) 
- [ ] [Create Github account](https://github.com/join) 
- [ ] [Download and install github's command line tools](https://help.github.com/articles/set-up-git/#setting-up-git) 
- [ ] [Download and install Node.js ](https://nodejs.org/en/download/) 
- [ ] Download and install a text editor (I recommend [sublime text 3](https://www.sublimetext.com/3))

##### 1. Make a copy of my existing project on github by forking the project at https://github.com/zsobin/BaseWebApp.git
<img width="400" alt="github" src="https://cloud.githubusercontent.com/assets/17851174/25285298/b990a2ae-2687-11e7-845c-2673aa704689.png">

##### 2. Find and open your terminal 
<img width="115" alt="screen shot 2017-04-21 at 11 43 48 am" src="https://cloud.githubusercontent.com/assets/17851174/25285319/ce48dafe-2687-11e7-9fba-3262f406235f.png">

##### 3. Use the command line to navigate to your desktop:
- `ls` lists all files in a directory. If you're on a PC, the command is `dir` instead. 
```
	cd ~/Desktop 
	ls 
```
you should see all the items on your desktop displayed in text in the terminal like so: 
![oct-12-2016 21-51-18](https://cloud.githubusercontent.com/assets/17851174/25285297/b97b3586-2687-11e7-8d0a-075baed899c4.gif)

 
##### 4. Fork the Repository 

When you create (or in this case, fork) a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations. Use the command line to (1) clone your project from Github onto your own computer, then (2) navigate into the project and then (3) list all the files in the project:

```
	git clone https://github.com/YourUserName/BaseWebApp.git 
	cd BaseWebApp
	ls
```

##### 5. Initialize app for Heroku

Use the command line to create an app on Heroku, which prepares Heroku to receive your source code (and initializes a url for you) 
```
	heroku login
	heroku create
```

##### 6. Install dependencies

Install the project’s dependencies using npm, a tool used to install any other projects your project needs in order to run locally. View the dependencies your app needs here.
```
	npm install 
```

##### 7. Run the project on your machine (your local server)
```
	heroku local web	
```

##### 8. Link github repo to heroku
 - Go to https://dashboard.heroku.com/apps
 - Select your app
 - Click the tab ‘Deploy’ 
 - In Deployment Method, select ‘Connect to Github’ and follow instructions to connect

##### 9. Make a change in the code

Open the project with Sublime text or whichever text editor you installed. Make a change to your code (ex. In index.ejs change the header text)

##### 10. Push that change to github (which automatically deploys on Heroku)
```
	git add .
	git commit -m “made my first change!” 
	git push origin master
```

##### 11. View your app live! (it might take a few seconds to finish deploying)
```
	heroku open 
```	

### Phase 2 - Continue to work off of ‘Hello World’ 

- [Option 1 - Personal website](https://github.com/zsobin/PersonalWebApp): This is the easier option, using only HTML and CSS. 
- [Option 2 - Incorporate database](https://github.com/zsobin/DatabaseWebApp): this is more challenging, and only recommended for attendees who are familiar with HTML, CSS and a little bit of javascript. 	

Step-by-step instructions for these can be found in the repo READMEs. 
