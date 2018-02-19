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

*Note: on Windows, it might be called Git Shell or Git BASH.*

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

*Note: On Windows, the first command might 'hang' for quite some time (even up to 10-15 minutes) - do not cancel and restart it, usually after this first 'long' run, it works without issues later on.*

If you experience any issues with Heroku CLI, please refer to https://devcenter.heroku.com/articles/heroku-cli#troubleshooting and your error log file.

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

Few editors that you might find helpful:
* [Sublime Text](https://www.sublimetext.com/) - free to evaluate, but requires licence if you plan to use it every day
* [Atom](https://atom.io/) - completely free editor
* [Visual Studio Code](https://code.visualstudio.com/) - another free to use editor

In fact, any text editor will  work - if you have favourite one, please use it!

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
	git commit -m “made my first change” 
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

### Additional materials

To help you with further development, we’ve gathered together some additional materials. Hope you will find them useful.

**Git and GitHub tutorials**
Version control is an important tool for every developer, and git is the most popular one. Learn more [useful git commands](https://try.github.io/levels/1/challenges/1), discover [the branching]( https://learngitbranching.js.org/) and then check [how to use GitHub](https://guides.github.com/activities/hello-world/) for your own project.

**Web App tutorials (HTML, CSS, JavaScript)**
There are plenty of different tutorials and online resources to learn HTML, CSS and JavaScript. We have found these useful and interactive:

- FreeCode Camp interactive web development tutorial: https://www.freecodecamp.org/ 
- Khan Academy free html and css tutorial: https://khanacademy.org/computing/computer-programming/html-css 
- Comprehensive web development tutorial/documentation by Mozilla: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web

 - CSS visual guide: https://cssreference.io/ 
- Flexbox tutorial: http://flexboxfroggy.com/ 
- cssGrid tutorial: http://cssgridgarden.com/ 

- HTML cheatsheet: http://www.hostingreviewbox.com/html5-cheat-sheet/

**Inspiration and problem solving**
To practice your problem solving skills and find some inspiration, please check the following pages: 
- [StackOverflow](https://stackoverflow.com/) is a great place to ask any question (or search for it first, because it’s very likely that someone has already asked the same question and got an answer :))
- [Code Pen](https://codepen.io/) is a great source of inspiration with a lot of projects based on HTML, CSS and JavaScript
- [Dev.to](https://dev.to/) is a blog platform where you can find plenty of useful posts from other developers.
