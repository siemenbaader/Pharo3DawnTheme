Pharo3DawnTheme
===============

Pharo3DawnTheme is a dark, Sublime-inspired theme for Pharo 3 by Sebastian Sastre, based on Esteban Lorenzano's Pharo3DarkTheme.

I have updated the installation instructions to work with Pharo 4.0 and that is all I have done.

-- [Siemen Baader](https://github.com/siemenbaader)

##Screenshot

![Pharo 3 Dawn Theme Screenshot](https://raw.githubusercontent.com/siemenbaader/Pharo3DawnTheme/master/img/screenshot.png)

##Installation instructions for Pharo 4.0

*If your Pharo isn't able to do github already:*

        Gofer new 
            url: 'http://smalltalkhub.com/mc/Pharo/MetaRepoForPharo40/main';
            configurationOf: 'GitFileTree'; 
            loadStable.

Then:
        
        | repo |
        
        repo := MCFileTreeGitRepository fromZnUrl: (ZnUrl fromString: 'gitfiletree://github.com/siemenbaader/Pharo3DawnTheme.git?protocol=https&dir=src&branch=master').
        Gofer it
    		repository: repo;
			package: 'Pharo3DawnTheme';
			load.
		
		(Smalltalk at: #Pharo3DawnTheme) installFullTheme.
	

###*Pharo Smalltalk
Getting a fresh Pharo Smalltalk image and its virtual machine is as easy as running in your terminal:
 
    wget -O- get.pharo.org/40+vm | bash

_______

MIT - License

2014 - [sebastian](http://about.me/sebastianconcept)

o/
