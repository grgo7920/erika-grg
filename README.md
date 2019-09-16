# WLU - CP202
This repository contains all the code and lectures for CP202 (Fall 2019).

If you have any questions, email jsandoval@wlu.ca.

# Running Locally - Part 1 of Quiz 1
The following steps will help you set up the software required to run locally. 

Setting up the site to run locally counts as 2.5% of your total mark as part 1 of Quiz 1 (the total weight of Quiz 1 is 5%). 

The first time you run the site locally, you will get instructions to submit validation that it is running in your machine.

## Step 1

You need to clone the repository using git. You may already have git installed. To verify you have it installed, run the following command:
```
$ git --version
```

If you get something that looks like the following, you're all set (go ahead an clone the repo):
```
git version 2.12.2
```

If you need to install git, you have different options. In Mac OS X the very first time your run git, if not installed, the OS will give you the option to install it (follow the instructions).

For a different OS, use the appropriate installer from here https://www.atlassian.com/git/tutorials/install-git.

When you're done installing and verifying that it runs properly, clone the repository with the following command (you can choose any convinient directory--for my machine, I chose /User/jose/Documents):

```
$ cd /Users/jose/Documents
$ git clone https://github.com/josefelixsandoval/wlu.git
```

## Step 2
If you already have a web server installed in your machine, go to Step 3.

To run a local web server you have multiple options. I'll give you two (pick only one).

**Option 1: Python Built-in Web Server**\
If you are running MacOS (or have Python installed in your Windows machine), Python comes with a built-in web server.

Go to your desired directory and check which version of Python version you are running by using the following command:

```
$ python --version
```

If your version of Python is 2.7, you'll get an output similar to this:

```
Python 2.7.10
```

If you don't have python installed and would like to use the built-in server, install the latest version of Python and then run the command for 3.7. You can find the latest version here https://www.python.org/downloads/ (this works for Windows and MacOS).

**Option 2: Node.js Web Server**\
If you have Node.js and the http-server module already installed, skip the installation part and just run the http-server command as listed in item 3 here.

To install Node.js:

1. Go to https://nodejs.org/en/download/ and download and install it.
2. Open a shell terminal or command prompt (in Windows) and install http-server with the following command:

```
$ npm install http-server -g
```

3. Run the following command after you are in your desired directory.

Go into the directory where yo downloaded the repository

```
$ cd /User/jose/Documents/wlu/www
```

And then run the server:

```
$ http-server -p 8000
```

To view your local web server, point your browser to the following URL:

```
http://localhost:8000/index.html
```

**NOTE: off the box, http-server will not serve 'index.html' as the default file. Just add 'index.html' to your URL.**

## Step 3
After you have cloned this repository, go to the root directory of the repo and run your prefered web server. For example, my local version of the site is in the following directory:

```
$ cd /User/jose/Documents/wlu/www
```

Then run the following command if you have Python version 2.7:

```
$ python -m SimpleHTTPServer
```

If Python version is 3.7, then run the following command:

```
$ python -m http.server
```

You then can view your local website by going to the following address in your web browser:

```
http://localhost:8000/
```

You should see the homepage for the site. I'll be updating it weekly, but it should look something like this:

![Home Page](http://wlu-cp202.appspot.com/img/homepage.png)
