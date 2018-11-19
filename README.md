

Overview:
========
The goal is to gather all initial setups for sublime, python, bash and git for personal use. 


Items:
=====
Following bash setting are borrowed from Corey Schafer's [dotfiles](https://github.com/CoreyMSchafer/dotfiles) github and with minor changes adopted (simplified) for personal use:

	.bash_profile
	.bash_prompt
	.gitignore


Sublime Text 3 setup is inspired by [awesome series of sublime text tutorials](https://www.youtube.com/watch?v=zVLJfrIwEP8&list=PL-osiE80TeTtHH8BZngXEsLPGotQxZa6z) by Corey Schafer and [video course](ttps://training.realpython.com/courses/sublime-python/) by Daniel Bader.



Sublime Text 3 Setup 
====================

Prerequisites:
-------------
* Install Sublime Text 3
* Install Package Control 
* Install python3 and flake8 package
* Install Git


Sublime Package List:
---------------------
	Package Control

	Anaconda
	SublimeLinter
	SublimeLinter-flake8
	
	GitGutter

	MarkdownPreview

	BracketHighlighter
	SideBarEnhancements
	Zen Tabs

	Boxy Theme
	Tomorrow Color Schemes (needs to be installed before below package)
	Tomorrow Night Italics Color Scheme


Configure Git commit messages
-----------------------------
Tutorial on how to white a [good commit messages](https://chris.beams.io/posts/git-commit/) by Chris Beams.


**Note** Don't forget to configure user.name and email prior to configure commit messages with sublime:

	Set your username: git config --global user.name "FIRST_NAME LAST_NAME"
	Set your email address: git config --global user.email "MY_NAME@example.com"

**Link _subl_** On mac, it would be useful to create a link to sublime:
	$ ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl


To change the text editor used by git commit (assuming _subl_ command is linked to SublimeText3)
	
	$git config --global core.editor "subl --wait --new-window"


To add ruler specific to git commit messages (actually two rulers)
	
	1. open commit message in sublime
	2. Pref -> Settings Syntax-Specific 
		{
			"rulers": [50, 72]
		}



Customize Fonts
---------------

		- select and download fonts (e.g. ubuntu mono font)
		- install font on system level
		- add some options to subl settings, eg.:

			{

				"font_face": "Ubuntu Mono",

				"font_options":[
					"subpixel_antialias",
					"no_bold",
					"no_italic",
				]
			}

**Optional: Download and install Font (Source Code Pro)**

		
		$ wget -O ~/Downloads/source-code-pro.zip https://www.fontsquirrel.com/fonts/download/source-code-pro
		$ unzip ~/Downloads/source-code-pro.zip -d ~/Downloads/scp
		$ rm ~/Downloads/source-code-pro.zip

		(ubuntu)sudo apt update && sudo apt -y install font-manager

		Next, Add new font with Font Manager (mac, ubuntu)


Sublime Text 3 Frequently Used Commands:
========================================
For Multi-line Editing:

	ctr + cmd + cursor ...
	ctr + cmd + G 
	cmd + D 
	select items: cmd + Shift + <- or ->  ;  copy -> paste 
	cmd + W : close tab
	cmd + shift + T reopened recently close tab

