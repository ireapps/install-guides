# NICAR 2018 install guide

Drop by our [install party](https://www.ire.org/events-and-training/event/3189/3588/) at 10:15 a.m. on Sunday, March 11, in Clark, and we'll help you get your rig set up.

![ow wow](gifs/judgejudy.gif "judge judy can't even with this")

_Meantime_, Here's how IRE set up the PC and Mac laptops for #NICAR18. (Keep in mind that you may not need _all_ of these tools at once.)

A note on Python packages: To simplify things, we didn't use virtual environments to isolate dependencies for each Python session. You should do this for your projects, though! A variety of tools can help you manage project dependencies in a virtual environment, including [pyenv](https://github.com/pyenv/pyenv), [pipenv](https://pipenv.readthedocs.io/en/latest/) and [virtualenv](https://virtualenv.pypa.io/en/stable/) (plus, optionally, [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/)). (The conference computers have `virtualenv` and `virtualenvwrapper` available, FWIW.)

Also, we didn't include instructions for setting up a virtualbox to run the programs used in the ["CAR Throwback" session](https://www.ire.org/events-and-training/event/3189/3666/). (If you really get the urge to party like it's 1998, let us know and we'll hook you up.)

## Windows

- [Microsoft Office](https://www.office.com/): Word, Excel, Powerpoint, Access
- [VLC Media Player](http://www.videolan.org/vlc/index.html)
- [Python 3.6.4](https://www.python.org/downloads/) (Make sure that the "Install launcher for all users" and the "Add Python 3.6 to PATH" checkboxes on the install screen are checked)
- Python packages:

  ```beautifulsoup4 ipython requests csvkit csvdedupe probablepeople usaddress sklearn pandas matplotlib lxml jupyter xlrd html5lib csvmatch matplotlib seaborn visidata pyshp coverage freezegun flake8 numpy nltk spacy tabula-py pypdfocr```

- [Node.js 8.9.4](https://nodejs.org/en/download/)
- Install some node packages globally (again, you probably won't need all of these installed for every project you do in life, so def take advantage of node's package management workflow to handle project dependencies):

  ```npm install -g gulp gulp-cli grunt grunt-cli http-server hot-server yo generator-yeogurt```

- [Flash](https://get.adobe.com/flashplayer/)
- [Java](https://java.com/en/download/)
- [Google Chrome](https://www.google.com/chrome/browser/desktop/)
- [Firefox](https://www.mozilla.org/en-US/firefox/new/)
- [R](https://www.r-project.org/)
- [RStudio](https://www.rstudio.com/)
- Install R libraries:

  ```"tidyverse", "fivethirtyeight", "nycflights", "babynames", "XML", "rtweet", "splines", "gee", "lme4", "nlme", "survival", "Ecdat", "DT", "here", "evaluate", "digest", "highr", "Rcpp", "htmltools", "knitr", "rprojroot", "rmarkdown", "leaflet", "shinycssloaders", "rgdal", "tigris", "packrat"```

- [MiKTeX](https://miktex.org/) ([follow these instructions](https://miktex.org/howto/install-miktex))
- [Neo4j](https://neo4j.com/)
- [Notepad++](https://notepad-plus-plus.org/)
- [QGIS 2.14](http://qgis.org)
- [git](https://gitforwindows.org/) ([setup guide](https://help.github.com/articles/set-up-git/))
- [PSPP](https://www.gnu.org/software/pspp/)
- [DB Browser for SQLite](http://sqlitebrowser.org/)
- [OpenRefine](http://openrefine.org/)
- [Tabula](http://tabula.technology/)
- [Postman](https://www.getpostman.com/)
- [The Tableau Reshaper Tool for Excel](https://community.tableau.com/servlet/JiveServlet/download/10394-2-178585/tableau_data_tool.zip) (ZIP)
    - Once the file is on your computer, extract the file from the ZIP file and double-click it to install
    - Open Excel, click the File tab, click Options, and then click Add-Ins
    - From the Manage box, select Excel Add-ins, and then click Go
    - In the Add-Ins dialog box, verify the check box next to the Tableau add-in is selected, and click OK
- [Sublime Text](https://sublimetext.com/)
- [atom](https://atom.io/)
- [GIMP](https://gimp.org/)
- [ArcGIS for Office](https://doc.arcgis.com/en/maps-for-office/install-and-configure/about-esri-maps-for-office.htm)
- [pdftk](https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit/)
- [cometdocs desktop app](https://www.cometdocs.com/)
- [tesseract](https://github.com/UB-Mannheim/tesseract/wiki)
- [ghostscript](https://www.ghostscript.com/)
- [imagemagick](http://imagemagick.org/script/index.php)
- [xpdf tools](https://xpdfreader-dl.s3.amazonaws.com/XpdfReader-win64-4.00.01.exe) (ZIP)
    - Extract the folder to a directory somewhere
    - Add the path to the `bin64` folder to the Environmental Variable path:
        - Right click on "This PC"
        - Click Properties, then Advanced System Settings
        - Click Environmental Variables
        - Select Path and click Edit
        - Add the path to the `bin64` folder you extracted, ensuring that you separate the path from the rest of the values in Path with a semicolon, then press OK
- [WAMP](http://www.wampserver.com/en/)
- Postgres and PgAdmin - check out this [@charlesminshew](https://github.com/charlesminshew) [installation guide](https://www.dropbox.com/s/bdvs6gglfu6hopv/PostgresWindowsInstallation.pdf?dl=0)
- [MySQL Web Community Installer](https://dev.mysql.com/downloads/installer/)
    - Choose the "Developer Default" install option
    - It will begin to check for requirements. The requirement for MySQL For Excel is the Microsoft Visual Studio Tools for Office Runtime 2010 setup.
    - A screen with a list of the products to be installed will appear. If you see this, press Execute, then Next, then Next
    - On the next screen, select Standalone MySQL Server / Classic MySQL Replication
    - Click Next. On the next screen, choose "Development Machine" for Config Type. Make sure that the checkboxes next to TCP/IP and Open Firewall port for network access are checked. Set the Port Number to 3306 (default)
    - Click Next. On the following screen, set the MySQL Root Password and make a note of it somewhere. Do not add any user accounts, for now.
    - Click Next. Check the boxes to Configure MySQL Server as a Windows Service and allow the default name to persist. Also check the box to Start the MySQL Server at System Startup. Run the Windows Service as a Standard System Account by selecting the button next to that option.
    - Once you click Next, you'll see a screen for Plugins and Extensions. Do not do anything on the page when asked to change settings for MySQL as a Document Store. Click Next.
    - On the next screen, press Execute to apply the configuration. Then click Finish. You’ll be back at the Product Configuration screen. Press Next.
    - On the MySQL Router Configuration screen, do not make any selections. Simply click Finish.
    - You will then see a screen to Connect to Server. Make sure MySQL Server 5.7.21 has a checkbox marked next to it. Supply the credentials below that. Username is root and password is whatever password you set earlier. Press Check to see if the connection was successful. 
    - Click Next. On the following screen, press Execute. You'll see a screen indicating the Installation is complete. Click Finish.

## Mac

- [Microsoft Office](https://www.office.com/): Word, Excel, Powerpoint
- [Flash](https://get.adobe.com/flashplayer/)
- [Java](https://java.com/en/download/)
- [Google Chrome](https://www.google.com/chrome/browser/desktop/)
- [Firefox](https://www.mozilla.org/en-US/firefox/new/)
- [VLC Media Player](http://www.videolan.org/vlc/index.html)
- [Filezilla](https://filezilla-project.org/)
- [Homebrew](https://brew.sh/) -- in your terminal, run:

  ```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

- In your terminal, run: `xcode-select --install`
- Brew install python3, git, node, tesseract, xpdf, imagemagick, ghostscript:

  ```brew install python3 git node tesseract xpdf imagemagick ghostscript```

- Python packages:

  ```beautifulsoup4 ipython requests csvkit csvdedupe probablepeople usaddress sklearn pandas matplotlib lxml jupyter xlrd html5lib csvmatch matplotlib seaborn visidata pyshp coverage freezegun flake8 numpy nltk spacy tabula-py pypdfocr```

- Install some node packages globally (again, you probably won't need all of these installed for every project you do in life, so def take advantage of node's package management workflow to handle project dependencies):

  ```npm install -g gulp gulp-cli grunt grunt-cli http-server hot-server yo generator-yeogurt```

- [MAMP](https://www.mamp.info/en/)
- [Tabula](http://tabula.technology/)
- [R](https://www.r-project.org/)
- [RStudio](https://www.rstudio.com/)
- Install R libraries:

  ```"tidyverse", "fivethirtyeight", "nycflights", "babynames", "XML", "rtweet", "splines", "gee", "lme4", "nlme", "survival", "Ecdat", "DT", "here", "evaluate", "digest", "highr", "Rcpp", "htmltools", "knitr", "rprojroot", "rmarkdown", "leaflet", "shinycssloaders", "rgdal", "tigris", "packrat"```

- [Postgres app](http://postgresapp.com/)
- [Postman](https://www.getpostman.com/)
- [Neo4j](https://neo4j.com/)
- [MacTeX](http://www.tug.org/mactex/)
- [QGIS 2.14](http://qgis.org)
- [PSPP](https://www.gnu.org/software/pspp/)
- [DB Browser for SQLite](http://sqlitebrowser.org/)
- [OpenRefine](http://openrefine.org/)
- [Sublime Text](https://sublimetext.com/)
- [atom](https://atom.io/)
- [GIMP](https://gimp.org/)
- [pdftk](https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit/)

## More in-depth installation guides

- [NYT: Set up your Mac like an interactive news developer](https://open.nytimes.com/set-up-your-mac-like-an-interactive-news-developer-bb8d2c4097e5)
- [NPR: How to setup your Mac to develop news applications like we do](http://blog.apps.npr.org/2013/06/06/how-to-setup-a-developers-environment.html)
- [The Hitchhiker's Guide to Python](http://docs.python-guide.org/en/latest/)
- [Anthony Debarros: Setting up Python in Windows 10](http://www.anthonydebarros.com/2015/08/16/setting-up-python-in-windows-10/)