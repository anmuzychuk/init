

Overview:
========
The goal is to gather all initial setups for sublime, python, bash and git for personal use. 


Items:
=====
Following bash setting are borrowed from Corey Schafer's [dotfiles](https://github.com/CoreyMSchafer/dotfiles) github and with minor changes adopted (simplified) for personal use:

	.bash_profile
	.bash_prompt
	.gitignore


Sublime Text 3 setup is inspired by awesome [series of tutorials by 
Corey Schafer](https://www.youtube.com/watch?v=zVLJfrIwEP8&list=PL-osiE80TeTtHH8BZngXEsLPGotQxZa6z) and [video course by Daniel Bader](https://training.realpython.com/courses/sublime-python/).



Sublime Text 3 Setup 
====================

Prerequisites:
-------------
* Install Sublime Text 3
* Install Package Control 
* Install python3 and flake8 package 


Sublime Packages:
-----------------
	Package Control
	Anaconda
	Boxy Theme
	BracketHighlighter
	GitGutter
	SideBarEnhancements
	SublimeLinter
	SublimeLinter-flake8
	Tomorrow Night Italics Color Scheme
	Zen Tabs




Configure Git commit messages:
-----------------------------

Tutorial on how to white a good commit messages by [Chris Beams](https://chris.beams.io/posts/git-commit/)


# change the text editor used by git commit 
git config --global core.editor "'/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl' --wait --new-window"

# to add ruler specific to git commit messages (actually two rulers)
	
	1. open commit message in sublime
	2. Pref -> Settings Syntax-Specific 
		{
			"rulers": [50, 72]
		}


# link subl
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl


# Example to customize fonts
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





Sublime Text 3 Frequently Used Commands:
========================================
For Multi-line Editing:

	ctr + cmd + cursor ...
	ctr + cmd + G 
	cmd + D 
	select items: cmd + Shift + <- or ->  ;  copy -> paste 
	cmd + W : close tab
	cmd + shift + T reopened recently close tab

