---
description: This tutorial will help you set up your git &  github account.
---

# Setting up git & github account

* Head to [github.com](https://www.github.com) and create your account. 
* Once you've created the account, you should see a dashboard like this. 

![github.com dashboard](../.gitbook/assets/screenshot-2019-01-13-at-2.56.54-pm%20%281%29.png)

* Click  "Your profile" from the menu. 

![github profile](../.gitbook/assets/screenshot-2019-01-13-at-2.57.04-pm.png)

* Go to "repositories" 

![github repos](../.gitbook/assets/screenshot-2019-01-13-at-2.57.11-pm.png)

* You can see a list of your repos here. Since you'll be setting this for the first time, click on new to add a repo. 

![creating a new github repo](../.gitbook/assets/screenshot-2019-01-13-at-2.57.28-pm.png)

* Give a repo name - think of it as a folder name in your pc
* Add description \(optional\)
* Check whether you'd like your repo public or private. For this tutorial, we are going to make a public repo. 
* Check the "Initialize this repository with a README" 
* Click on "Create repository" 

![new repo](../.gitbook/assets/screenshot-2019-01-13-at-2.57.42-pm.png)

 

* You've successfully created your first repo. We have a file called README already in the repo. Now we'll look to have something added to the file and commit it to the repo. 
* Before that, you need to setup git in your pc.

## Setting up git

* Click [here](https://git-scm.com/downloads) to go to the git download page. Choose your platform \(Mac, Windows/ Linux\) and click download. 
* Once the file is downloaded, install the program.

![git installation successfully completed ](../.gitbook/assets/screenshot-2019-01-13-at-3.24.33-pm.png)

* Open terminal\(mac, linux\)/ command prompt \(windows\) - In mac, search for "terminal" \| Windows user - "**Start** &gt;&gt; Program Files &gt;&gt; Accessories &gt;&gt; Command Prompt"  
* Use the command below to check your git version and to make sure that it has been successfully installed. 

```text
git --version
```

![git version command](../.gitbook/assets/screenshot-2019-01-13-at-3.28.35-pm.png)

Here you can see my git version in "_versions 2.20.1_" \(may vary from yours but that's fine\). 

* Now you are ready to use git in your pc

## Cloning github repo to your pc

> Think of cloning as copying a folder from your github account \(cloud\) to your pc \(local file\). Now the difference is, whatever change you make on you local pc flies can be selectively added to the cloud version using commit and push \(more on that later\). The advantage is that you don't need to overwrite the entire file to reflect a small change. Also other people can collaborate to make changes.

* Let's create a local folder in your pc and call it "tutorial" . I have created mine in the "documents" folder - I suggest you do the same to easily follow the rest of instructions. 
* Now open terminal and use the command below to navigate to the tutorials folder 

```text
cd Documents/tutorial/
```

![navigate to tutorial folder in terminal](../.gitbook/assets/screenshot-2019-01-13-at-3.48.22-pm.png)

* Go to your repos in github profile 

![](../.gitbook/assets/screenshot-2019-01-13-at-3.37.09-pm.png)

* Click on clone or download and select "Use HTTPS". 

![](../.gitbook/assets/screenshot-2019-01-13-at-3.37.23-pm.png)

* Copy the https link highlighted. 
* Use the "git clone" command to clone the learn folder to your tutorial folder in pc. 

```text
git clone <your repo link>
```

![cloning git repo](../.gitbook/assets/screenshot-2019-01-13-at-3.50.45-pm.png)

![clone successful ](../.gitbook/assets/screenshot-2019-01-13-at-3.50.57-pm.png)

* If everything's right you'll see something like above. You should now see a new folder named "learn" inside the tutorial folder. You have successfully cloned your learn repo to the tutorial folder. 

![Cloned learn folder in tutorial folder. ](../.gitbook/assets/screenshot-2019-01-13-at-3.51.09-pm.png)

* You can also see the README file inside the learn folder. 

![README file in learn folder. ](../.gitbook/assets/screenshot-2019-01-13-at-3.51.18-pm.png)

* Now to make our first commit \(change the local file and upload to cloud\), open the README file in a text editor. 
* Add a new line. 
* Save the file. 

![README.md](../.gitbook/assets/screenshot-2019-01-13-at-3.55.44-pm.png)

* Use the command line to navigate to our learn folder 

```text
cd learn
```

Now to add the changes \(stage\) use the command below.  - The "." indicates that all the changes to be added to the commit. 

```text
git add .
```

![git add](../.gitbook/assets/screenshot-2019-01-13-at-3.59.53-pm.png)

* Now we are about to commit the changes. 
* use the command below : The text inside " " indicate the commit message for easy understanding of the changes made and easy housekeeping for later. 

```text
git commit -m "my first commit. added a line in README.md" 
```

![](../.gitbook/assets/screenshot-2019-01-13-at-4.04.35-pm.png)

Note : You'll need to input your username and password for the push to happen. 

* Now we need to use the command below to push the commits to the cloud 

```text
git push
```

![Successful push](../.gitbook/assets/screenshot-2019-01-13-at-4.06.07-pm.png)

Congrats! You've successfully pushed your first commit to the github repo. 



![push changes reflected in the repo. ](../.gitbook/assets/screenshot-2019-01-13-at-4.07.18-pm.png)

