Download Link: https://assignmentchef.com/product/solved-cs2261-lab00-mac-installation
<br>
<h2>Provided Files, Folders, and Executables</h2>

<ul>

 <li>.vscode (folder)</li>

</ul>

○ tasks.json

<ul>

 <li>Makefile</li>

 <li>c</li>

 <li>Dockerfile</li>

 <li>visualboyadvance-m.app</li>

</ul>

<h2>Files to Edit</h2>

<ul>

 <li>tasks.json</li>

</ul>




<h2>Instructions</h2>

In this lab, you will be installing the software to write, compile, and run GBA games for this class. It is broken up into various parts. If any part does not produce the expected outcome, alert a TA via Teams and fix the problem before continuing. ​<strong>It is incredibly important that you read each and every instruction</strong>​. Many of your questions will be answered if you read carefully. Do not skim this document! &#x1f642;

<h3>Part 1: Docker Desktop</h3>

First, you’ll need to download Docker Desktop. In order to do this, you’ll need to sign up for Docker Hub. Sign up for Docker Hub here: ​<a href="https://hub.docker.com/signup">https://hub.docker.com/signup</a><u>​</u><a href="https://hub.docker.com/signup">.</a> You can use your personal or GT email; either is fine.

Once you’ve signed up, follow the detailed Docker Desktop download instruction here:

<a href="https://docs.docker.com/docker-for-mac/install/">https://docs.docker.com/docker-for-mac/install/</a>




Here, you’ll click on the “Download from Docker Hub” button (as seen above) and, granted you’re logged into the Docker Hub account you created, you’ll be taken to a new page that looks like the following:




Press the “Get Stable” button. In your downloads, you’ll see “Docker.dmg”.

Now, follow the “Install and run Docker Desktop on Mac” instructions on the Docker

Desktop download instructions page

<a href="https://docs.docker.com/docker-for-mac/install/#install-and-run-docker-desktop-on-mac">(</a><a href="https://docs.docker.com/docker-for-mac/install/#install-and-run-docker-desktop-on-mac">https://docs.docker.com/docker-for-mac/install/#install-and-run-docker-desktop-on-m</a><u>​   </u><a href="https://docs.docker.com/docker-for-mac/install/#install-and-run-docker-desktop-on-mac">a </a><a href="https://docs.docker.com/docker-for-mac/install/#install-and-run-docker-desktop-on-mac">c</a>)​ . Stop once you reach the “Uninstall Docker Desktop” section. Great, you’ve got Docker Desktop on your machine! &#x1f642; Go to your applications, and click Docker.app, as seen below.

You should see, in the top right of your screen, a little icon that looks like the following:




This icon indicates that Docker Desktop is running on your machine!​<strong> YOU MUST BE RUNNING DOCKER IN ORDER TO BUILD YOUR CODE</strong>​. Otherwise, when you attempt to build your code, you will see the following error:




If you see this, you’ll know you forget to open the Docker Desktop application.

<h3>Part 2: VisualBoyAdvance-M</h3>

Let’s get the GBA emulator setup! VisualBoyAdvance-M is the emulator for this class. If you already have a GBA emulator that you are comfortable with, I still highly recommend you use this one for this class. It has some special features that will come in handy for debugging.

Find the “​<em>visualboyadvance-m.app</em>​” application in the Lab00 folder in a folder parent folder. I recommend creating a parent CS2261 folder that will contain all of your homework, labs, etc. and keeping the “​<em>visualboyadvance-m.app</em>​” in this folder. Lab00 should be in this CS2261 folder, too. Keep a note of the exact path of the “​<em>visualboyadvance-m.app</em>​”. In the image below, you’ll see a recommended folder setup. The exact path to

<em>“visualboyadvance-m.app</em>​”, in this case, is

/Users/mariezimmy/CS2261/visualboyadvance-m.app




You can verify the directory location of the “​<em>visualboyadvance-m.app</em>​” on your machine by simply opening Finder, opening the CS2261 folder where you placed the

“​<em>visualboyadvance-m.app</em>​”, and dragging the “visualboyadvance-m.app” icon into the terminal. The output in the terminal is the exact path to the “​<em>visualboyadvance-m.app</em>​”. The sequence of images below shows this process.




In this case, as stated before, the exact path is

/Users/mariezimmy/CS2261/visualboyadvance-m.app​. Copy this exact path

and paste it into your task.json, on line 9 in between “open” and “./Project.gba”. Make sure there is a space after “open” and before “./Project.gba”. The (truncated) image below outlines what my tasks.json looks like. Your exact path on line 9 will be different! Remember to save your changes to your tasks.json file.




<h3>Part 3: Visual Studio Code</h3>

Visual Studio Code is the text editor of choice for this class. We highly recommend you use this editor. If you do not already have VSCode, you can download it here: <a href="https://code.visualstudio.com/download">https://code.visualstudio.com/download</a>​.

Once downloaded, open VSCode, and open the Lab00 folder by selecting File &gt; Open &gt; Lab00.

Open main.c and then hit ​<strong>cmd+shift+b </strong>​to build your project (remember, Docker Desktop needs to be running!). This first compilation process will take some time because a Docker image is being downloaded from Dockerhub (don’t worry about the nitty gritty details of this). ​<strong>All subsequent builds will not take this long </strong>​(whew). In the terminal output in VSCode, you should see something like this for the very first time you build:




Once the build is complete, you should see something like the following pop up:




If instead you get an error that that says you cannot open the visualboyadvance-m app, follow the instructions here to allow your Mac to open the application from an unidentified developer: <u>​</u><a href="https://support.apple.com/en-gb/guide/mac-help/mh40616/mac">https://support.apple.com/en-gb/guide/mac-help/mh40616/mac</a><u>​</u><a href="https://support.apple.com/en-gb/guide/mac-help/mh40616/mac">.</a> Then, try building again. You should see the image above.

If you do, congrats, follow the submission instructions &#x1f642; If not, recall, you need to have

Docker Desktop running to build your code! If this is not your issue, notify a TA via Teams.