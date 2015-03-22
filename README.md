# Welcome to the Docklands Dojo website project!

# Contributing

## Getting Started
Is this your first time working on the Dojo Docklands website?
Here's what you'll need installed on your computer:

(If you're a beginning coder, start at the top of this install list and work your way all the way to the bottom of the document. If you're anywhere else on the experience scale, start at the place where you're missing something and work your way down from there. You can skip the beginning bits.)

[**Installing the Environment and Languages**](#installing-the-environment-and-languages)

(start here if you're brand new to coding or missing one of the pieces of tech)

[Ruby](#ruby) | [Ruby Bundler](#ruby-bundler) | [XCode Command Line Tools](#xcode-command-line-tools) | [NodeJS](#install-nodejs) 

[**Installing Project-Specific Pieces**](#installing-project-specific-pieces)

(start here if you already have everything above installed)

[Jekyll](#installing-jekyll-and-github-pages) | [GitHub Pages](#installing-jekyll-and-github-pages)

**Getting the Project Onto Your Computer and Up and Running Locally**

[Forking and Cloning the Project](#getting-started---github)

[Setting Up Your Local Environment](#getting-started---setting-up-the-project-locally)

**Guidelines for Changing Code**

[Contributors' Guidelines](#guidelines)

# Installing the Environment and Languages

### Ruby
The Docklands Dojo website is built with Jekyll, which is dependent on some Ruby. Don't worry if you don't know Ruby - we will just be installing a couple of things on your computer so it can support Jekyll in the background.

First, let's check if Ruby is installed on your computer. It is on many Macs. You can do this by opening your Terminal and running this command:

```ruby -v```

If you don't get anything back, you will need to install Ruby.

1. First, let's install rbenv (which will help us install Ruby):
* Copy this line 

```git clone https://github.com/sstephenson/rbenv.git ~/.rbenv```

and paste it into your Terminal. Then hit 'Enter' to run the command.
* Then you're going to copy and paste this line

```echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile```

into the Terminal. Again, hit 'Enter' to run the command.
* Next, copy and paste this line into the Terminal:

```echo 'eval "$(rbenv init -)"' >> ~/.bash_profile```

Again, hit 'Enter' to run the command.
* These last two commands just configured some profile options for us. Don't worry too much about this right now. We're just getting you set-up.

2. Now open a new Tab in your Terminal. Type

```rbenv  ```

and you should see an rbenv version now.

3. We'll use the ruby-build plug-in to install Ruby. So to install this plug-in, copy and paste this line into your Terminal:

```git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build```

This will allow us to install Ruby.

4. Now we'll move on to installing Ruby itself.
* First let's check the current version of Ruby. We can find this at [Ruby-Lang.org](https://www.ruby-lang.org/en/downloads/)
* Finally, we can install this version of Ruby, by typing the command

```rbenv install 2.0.0-p353```

The version number is 2.0.0-p353. Your version number should be whatever the current Ruby-Lang.org docs say is the current version. Just replace the version number we've listed here when you're installing.

Don't worry if this takes a while! 

### Ruby Bundler
Next, let's make sure you have the Ruby Bundler installed on your computer. You can install it by copying and pasting the below line into your Terminal:

```gem install bundler```

Make sure to hit 'Enter' to run the command.

Bundler is a package manager for Ruby.
### XCode Command Line Tools
If this is your first time working with the Terminal (or you recently upgraded your Mac version), you may also need to install the X-Code Command Line Tools. 

If it is your very first time installing the XCode Command Line Tools, you will need to register as an Apple Developer first. Don't worry - there is no cost associated with registering as an Apple Developer! There is only a cost when you want to deploy apps. Again, we won't be working with the Developer tools here. They'll just be playing a background support role. 

1. Register in the Apple Developer Program
Remember - there's no cost for this stage of registration!

[Registration page](https://developer.apple.com/programs/start/standard/create.php)

2. Download the XCode Command Line Tools
 
[Download](https://developer.apple.com/downloads/index.action)

### Install NodeJS
The Docklands Dojo website is built with Jekyll, which is dependent on NodeJS. Don't worry if you don't know NodeJS - we will just be installing a couple of things on your computer so it can support Jekyll in the background.

First, let's check if NodeJS is installed on your computer. You can do this by opening your Terminal and running this command:

```which node```

If you don't get anything back, you will need to install NodeJS.

1. Install NodeJS

[Download and Install NodeJS](https://nodejs.org/)

# Installing Project-Specific Piece
### **Installing Jekyll and GitHub Pages**

1. To install Jekyll, simply run this command in your terminal:

```gem install jekyll```

Just copy and paste the above script into your Terminal and then hit 'Enter'.

2. GitHub Pages should install when you run the Bundler inside your project later.

## Getting Started - GitHub 
Now that your computer is set-up and ready to go, you can go ahead and Fork the DocklandsDojo project onto your personal GitHub repository.

1. Fork the project

2. Now on your own copy of the project, copy the git clone URL down on the righthand side of the page

3. In a Terminal, type

```git clone```

and then paste the clone URL in beside it before you hit 'Enter', like this:

```git clone https://github.com/fakeusername/fakeprojectname```

Tip: I always place all my projects inside a project file so I'm not cloning things to my Main Directory.

You can create a similar Projects folder by using this command:

```mkdir Projects```

To clone into there instead of your root (Main) directory, first 
'cd Projects' (this will allow you to go inside the directory)
and then run the above git clone command.
It will clone your copy of the Docklands Dojo folder into the Projects folder.

4. Wherever you're coming from, make sure to change directories and go into your Docklands Dojo folder.
From root, 

```cd docklands-dojo```

or you might have to go

```cd Projects```

and then 

```cd docklands-dojo```

Just make sure you're inside the Docklands Dojo folder before you go any further!

## Getting Started - Setting Up The Project Locally
Now that you have a copy of the project on your own local machine, we have to run a couple of commands to get all the right dependencies set-up.

1. First, we're going to generate a copy of the site using the following command:

```jekyll build```

2. Next, we have to switch from the main git branch of the project into the gh-pages branch (gh is short for GitHub).
You can do this by running this command:

```git checkout gh-pages```

3. Now, let's run

```bundle install```

in the Terminal.
This will install all of the project dependencies, like the Github Pages gem.

Hint: The first time I ran the bundle install on this project, my computer ran into a problem installing Nokogiri, and then cancelled installing the entire bundle. This can happen with some gems, so don't worry. 
I ran

```gem install```

to fix this. 
Once Nokogiri has installed, you will have to run 

```bundle install```

again, to install the rest of the dependencies bundler cancelled when it ran into the problem.

Don't worry about this second part of the step if your Terminal doesn't tell you it failed!

====
Now you can create your own branch and start editing the page!

1. From gh-pages branch, run this command:

```git checkout -b MY_FEATURE_NAME```

Replace MY_FEATURE_NAME with the name of the feature you are adding. For example, if you are adding a new page, you could call it something like NINJA_DANCING_INSTRUCTIONS.

Once you have finished the work on that feature, and you want to work on something for parrots, for example, you would commit your work from NINJA_DANCING_INSTRUCTIONS, submit a merge request and then go create a new branch for PARROTS_TALKING_INSTRUCTIONS.

### Guidelines

Make sure to use a new branch for each new feature.

### How To: Add a Page

See the [Add a Page docs](adding.md)

Thanks for contributing!