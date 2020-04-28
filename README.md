# Deploying a Simple react app  on github 

#What is this ? 
A following the tuto of <a href="https://dev.to/yuribenjamin/how-to-deploy-react-app-in-github-pages-2a1f">@yuribenjamin</a> for create and deploy and github

# The steps reminder

## Installing in our project folder
```
npm install gh-pages --save-dev
```

## create a repository in github 
I name this one my-app like the name of the react app create

## In the package.json
### at the beggining :
add this line with username is the name of the github account and reponame the name of the repository 
```
  "homepage": "https://username.github.io/reponame",
```

For this example mine was : 

```
  "homepage": "https://lailayana.github.io/my-app",
```

### in scripts
```
"scripts": {
//...
"predeploy": "npm run build",
"deploy": "gh-pages -d build"
}
```

### In the terminal of the project folder

```
git init
git remote add origin git@github.com:lailayana/my-app.git
npm run deploy
git commit -m "Your awesome message"
git push origin master

```

replace my name and the name of the repository with your data 


