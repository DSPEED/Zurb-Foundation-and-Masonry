ZurbFoundationMasonry / Direkt SPEED Framework Parts
=====================

This is based on a super rudimentary example of implementing Zurb's Foundation 4.0.4 (most recent at publish date) with jQuery Masonry that is called ZurbFoundationMasonry on github.

It is now a super Integration of Zurb : master and Masonry : master
You can simply checkout both repos from here or the Source Repos into the sources/ folder and then use our css/ds.zurb+masonry.css
You can adjust pathes in that css file if you whant a other folder structure then our

|dsframework
|
|------|Sources
|	   |---foundation
|	   |---masonry
|	   |---jQuery
|
|---|js
|
|
|---|css
|	|---ds.zurb+masonry.css
|
|---|shell
	|---addproject.sh // Initals new WebProject Creates Vagrant, Creates Local Git forks dsframework, Adds Virtual domain name to C:\Windows\system32\drivers /etc/hosts
	|---cleanup.sh // Delets unneeded Files out of the Sources for Produktion
	|---upsources.sh // Pushes changes of all Source Repos back to Em to Update em if needed
	|---bootstrap.sh // Vagrant inital deploy Script for dsframework


Additional Infos from the old Project
====================

Unfortunately since masonry is being used we must ignore the resizing of images for a hard-px based measurement. This is set up similarly where as the container shrinks in size the images will not resize but the columns will rearrange to accomidate, the new container will then center itself accordingly to avoid ugly margin issues on the right side of a column where images are missing. This is the best solution for integrating a masonry into a responsive framework (see pinterest site).

Applying the masonry call onto a 'large-12' container within foundation has the same effect though, it will automatically choose the first image as the base-width of a psuedo column when creating columns to fit inside of the container. More information about specifics can be found on the jQuery masonry website, http://masonry.desandro.com/.

I claim no ownership to any of the in folder sources contained files since it is a simple integration of two existing elements, Zurb's Foundation and jQuery Masonry.




Copyright
=====================

I claim ownership on all additional Files in This Project that are not owned by Zurb or Masonry!