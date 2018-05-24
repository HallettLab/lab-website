# Hallett Lab website

This repository houses the Hallett Lab website, which is shared among members through Github and hosted by Netlify. 

Lab members should keep their own pages current, as well as contribute to the lab news feed and update research themes and study systems as appropriate. 

## Initial set-up

1) Create a Github user name and share it with Lauren, who can add you to the Hallett Lab organization page and as a contributor to this site.

2) Install R and RStudio (and git, if using a PC)

3) Within R, install the package blogdown by running the following script in the console:
`install.packages("blogdown")`

then load the package using the script:
`library(blogdown)`

4) Install hugo. The blogdown function has a helper function to do this in R. Run the following script:
`blogdown::install_hugo()`

5) Clone the repository. Using the terminal, navigate to the location you would like the website folder stored in. Copy the web URL from the green "Clone or download" tab on the repository homepage, and clone it to your local drive by entering `git clone thewebURL` in the terminal. In this case, it would be:
`git clone https://github.com/HallettLab/lab-website.git`


## Updating a page

1) Open the hallettlab.RProj (always open the project file, don't just open individual files)

2) Pull! Always pull before you make changes, and before you push.  You can pull by clicking on the blue down button on the Git tab of RStudio.

Alternatively, you can pull updated files to your local drive by navigating to the lab website folder in the terminal, and entering:
`git pull`

3) Update the content on your page. Website files are typical markdown (.md) files, not Rmarkdown files. There is a handy markdown cheatsheet here: http://assemble.io/docs/Cheatsheet-Markdown.html

Use existing pages as a guide. Don't forget to use a double-space if you want a line break to appear in the rendered file. 

4) Preview your changes! You can do this by running the following script in the console:
`blogdown::serve_site()`

The website should appear in the Viewer tab of RStudio. You can open it in a browser by clicking on the arrow-to-browser icon on the upper left of the Viewer tab.

5) When you are satisifed, share your updates. 

First, pull again (using the blue down arrow on the Git tab). 

Second, add your changes. In RStudio, this can be done by clicking on the Staged checkbox in the Git tab.  

Third, commit your changes. Click on the Commit button in the Git tab, then add a message that succinctly describes your changes, and press Commit.  

Fourth, push your changes. Click on the green up arrow. It may ask you for your Github user name and password. 

## Creating a new page
If there is a page that is similar to what you want to create, it might be simplest to copy it using "Save As" and then make changes to reflect what you want. Alternatively, create a new .md file. One way to do this is to use the Addins drop down at the top of RStudio. 

If you are creating a news item, make sure to save it in the "news" folder (the Addins dropdown will default to "posts"), and date it such that it appears in the correct order on the site (hopefully the default of the current day will suffice!). 

For news items, please add the month and year at the top of the entry, preceded by four hashtags. Copy existing entries for formatting. 

For other items - order appears based on the date (newer items are higher up). So just create a dummy date that slots it into the appopriate place. 



