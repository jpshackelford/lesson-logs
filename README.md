# Introduction

Several high school students recently expressed interest in learning to code and I agreed to help by working on an interesting intial project. This page will log  project activities in case others wish to follow along.

# Prepare your environment

Those working on the project with me are currently all using a Mac so my instructions assume that is what you have. I will happy entertain pull requests for content aimed at helping Linux or Windows users.

1\.  If you don't have a http://github.com account, please create one. 

2\. Create a project using https://pages.github.com. 

We will be creating a website which will be your project log. The goal here is to track instructions for what we will be doing together so that others can benefit from the work you are doing. If done right, someone will be able to go to your site, following the instructions and reproduce your project. If you can explain what you are learning to others, then it will be clear that you have actually learned it. And by sharing your work with the world you will become part of a community of makers who will build on what you do and from whom you will in turn learn even more.

Come up with a nice title and create a first entry with today's date and which captures what we are doing below.

3\. Install [VSCode](https://code.visualstudio.com).   We will be using this for editing code. Once you have installed it, you will also want to [configure VSCode](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line) to start from the command line. If something goes wrong with this second step, don't worry about it. We can look at it together when we do our first Zoom session.

4\. Install [homebrew](https://brew.sh).  We will be using this to make installing other development tools you'll need on your mac much easier.

5\. Install Python 3. 

```
$ brew install python3
$ python3 -V
```

6\. Install the `mcpi` python library.

```
pip3 install mcpi
```

# Create a Minecraft Server w/ Spigot and the Raspberry Juice Library

This step we will skip for now. I have done this for you and will email credentials to the server. Later we will come back and do this together.

# Write you first program to test the plugin and connectivity.

1\. Create a new file with VSCode called `mcpi-test.py` and insert the content below.

```
from mcpi.minecraft import Minecraft

mchost = "" # replace this with the ip address I send via email
mc = Minecraft.create(mchost, 4711)
mc.postToChat("Hello Minecraft World")
```

2\. Login to the Minecraft server created in the previous section and once you have done so, run the program you just saved.

```
$ python3 mcpi-test.py
```
