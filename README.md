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


##### 4. Clone the Repository 
When you create (or in this case, fork) a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations. Use the command line to 
 - (1) clone your project from Github onto your own computer, then 
 - (2) navigate into the project and then 
 - (3) list all the files in the project:

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
Install the project’s dependencies using npm, a tool used to install any other projects your project needs in order to run locally. View the dependencies your app needs [here](https://github.com/zsobin/BaseWebApp/blob/master/package.json#L9). 
```
	npm install 
```

##### 7. Run the project on your machine (your local server)
```
	heroku local web	
```

##### 8. View the project running locally
Open a browser and navigate to `localhost:5000`


##### 9. Make a change in the code and refresh the page running at `localhost:5000`
Open the project with Sublime text or whichever text editor you installed. Make a change to your code (ex. In `index.ejs` change the header text) and refresh your web browser- you should see the change!

Ejs is a templating language that stands for embedded javascript. It's like HTML but with some special sauce mixed in so that you can add in a little javascript that gets compiled to HTML before it's send to the browser. We won't really be using it for anything other than HTML today though. 

##### 10. Link github repo to heroku
This is kind of a weird step but it's worth it- What this does is essentially connects your heroku app to a Github Repository. It monitors the repository and whenever it sees you push a change, it automatically re-deploys your application so that your changes are incorporated in your live site. 

 - Go to https://dashboard.heroku.com/apps
 - Select your app
 - Click the tab ‘Deploy’ 
 - In Deployment Method, select ‘Connect to Github’
 - Search for your Repo- "BaseWebApp"
 - Click 'connect' and then 'Enable Automatic Deploys'
 
_*We use automatic deploys at HubSpot - but ours go to a 'QA' or 'staging' site. Can you think of why we might do that? Ask a hubspotter near you what they think!_

##### 11. Push that change to github (which automatically deploys on Heroku)
*If your server is still running from before (it probably is), you can press control + c to halt it

```
	git add .
	git commit -m “made my first change!” 
	git push origin master
```

##### 12. View your app live! (it might take a few seconds to finish deploying)
```
	heroku open 
```	

### Phase 2 - Continue to work off of ‘Hello World’ 

A few tips before you begin:
 - **Test often**- when you make a change, make sure it works. You don't want to add a bunch of stuff and spend tons of time tracking a little thing down.
 - **Google everything!** - Google is a developers best friend. I'm not joking. No one actually just _knows_ this stuff... you just get really good at knowing what to google and reading/incorporating the answers you find. 
 - **Ask for help** - Everyone around you is dying to help you out! Don't be afraid to ask, no matter how silly you think your question is (because trust me, it's not). 

 [Option 1 - Personal website](https://github.com/zsobin/PersonalWebApp): This is the easier option, using only HTML and CSS. 

 [Option 2 - Incorporate database](https://github.com/zsobin/DatabaseWebApp): this is more challenging, and only recommended for attendees who are familiar with HTML, CSS and a little bit of javascript. 	

Step-by-step instructions for these can be found in the repo READMEs. 
