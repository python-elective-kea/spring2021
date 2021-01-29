# Installations
This document will describe what you should install in order to follow this elective.   

You will not install python dirrectly on your computer, but instead throughout this semester run docker containers build opon different kinds of python images.    

The benifit of this appcoach is that we all, no matter what OS we normally use, can use the exact same development enviroment. This also makes it easier to work together across diffenret OS in groups. It also will teach you how to work with an industry standart, so you know this development environment and approach when you start to work after your education has ended.  

You probably already have installed some of the following applications, but if you do not you should now install:

1. Docker desktop 
2. Some kind of text editor.
3. Git 
4. Create a GitHub account.

## 1. Docker Desktop
### Download and install Docker Desktop

Navigate to the Docker website and download and install Docker Desktop for your operating system.   

[Docker Desktop download](https://www.docker.com/products/docker-desktop)    

#### Check if everything is installed
In your terminal or powershell you should type ``` docker --version ``` and get the following result.

````
	$ docker --version
	Docker version 19.03.8, build afacb8b

````
If you do not see this, get an error or like, then you still de not have docker installed on your system.

### Run your first Docker container (Ubuntu). 

The first Image you should create a container from is a basic Ubuntu image.    

Run the following command in your termianl to download the image and run a container.


````
	$ docker run -it --rm ubuntu
````
With:   

* ** -it **: you specify to run the container in interactive mode (you can use its terminal).
* ** --rm **: you specify that the container should be deleted when you exit the terminal.
* ** ubuntu ** : is the name of the image
 
After downloading has finnished, and run has executed you should see something like this in your terminal.

````
	$ docker run -it --rm ubuntu
	root@710ef1a882be:/#
````

Now you have a ubuntu operating system running on your computer (in a docker container).


### Run your Second Docker container (Python). 

The second Image you should create a container from is an official python docker image.    

Run the following command in your termianl to download the image and run a container.


````
	$ docker run -it --rm python bash
````

With:   

* ** -it **: you specify to run the container in interactive mode (you can use its terminal).
* ** --rm **: you specify that the container should be deleted when you exit the terminal.
* ** python **: is the name of the image.
* ** bash **: specifies that you want to start the container with a terminal gui (bash) 

After downloading has finnished, and run has executed you should see something like this in your terminal.

````
	$ docker run -it --rm python bash
	root@a7991e5db4cd:/#
````

Now you have an linux operating system running on your computer with some version of python installed in it (in a docker container).   

In the terminal you now have open type in the following:    

````
python --version
````

When pressing enter, you should now see the following

````
python --version
Python 3.8.2
````

## 2. Download and install a text editor (VS Code)
Download and install a text editor. There are many good ones, and you need at least one, but you decide which one.   

A good option is VS Code. You can download it from the following source: 

* [https://code.visualstudio.com/](https://code.visualstudio.com/)


## 3. Git & Github
### Download and install Git
* If you do not already have git installed on your computer you should do this now. 

* [https://git-scm.com/](https://git-scm.com/) 

_If you are on **Windows** be sure to install the "Git Bash" (this is an option you can choose during the installation process.)_

#### Check if everything is installed
* Open you terminal and type in the following

````
git --version
````
When pressing enter, you should now see the following

````
git --version
git version 2.10.1  // or some other version number
````

If you see something else, Git is not installed correct, and you should try again.


## 4. Create a Github Account
* If you do not already have a GitHub account, you should create one now. 
    * Go to https://github.com/ and create an account 


