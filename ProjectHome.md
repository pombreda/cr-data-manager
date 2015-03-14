# crDataMan: The ComicRack Data Manager #

### docdoom & T3KN0Gh057 proudly present the CR Data Manager ###

If you are using ComicRack for Windows to organize your comic library there is sometimes the need to enter data based on rules. So you might want to set the series group to Gotham for all Batman books. Or you scraped your data from ComicVine (using the excellent ComicVine Scraper) and discover that some of the information in the ComicVine database is not correct. So you want to set the publisher information in your library for the first 200+ issues of Walt Disney's Comics & Stories to Dell instead of Boom. This plugin will complete all these tasks automatically.

**See the [manual](http://code.google.com/p/cr-data-manager/downloads/list) for more information about installation and usage. If you would like to discuss the Data Manager you are invited to do so at this [thread](http://comicrack.cyolito.com/forum/13-scripts/33002) at the ComicRack forum.**

**Please note:** Data Manager works best if you scraped your books before with the excellent and highly recommended [ComicVine Scraper](http://code.google.com/p/comic-vine-scraper).

## Important: version 1.2 is now released (2013-06-14) ##

Major changes in this version:

  * The Data Manager is much faster now (factor 40 compared to version 1.1)
  * delimiter for multiple list items has changed from comma to '||' (but you don't have to worry about it, the GUI will do that for you for your current ruleset collections)
  * 'OR' mode for rules implemented
  * new modifiers ContainsAllOf, NotContainsAllOf, NotRange
  * if a field is changed by one ruleset but multiple actions only the last value is written to the logfile
  * the GUI supports searching the ruleset collection for any field, modifier or value

Changes in version 1.1:
  * You don't need to write any text-based rules anymore. The previous editor has completely been replaced by a graphical interface which makes it much easier to create your rules.
  * Organization of your rules in groups in an explorer-like interface
  * Creation of rule templates
  * Now a nearly complete set of all ComicRack fields can selected/manipulated with the Data Manger.
  * A lot of new modifiers have been added.

**You can download the installation [here](http://code.google.com/p/cr-data-manager/downloads/list).**

**Please note:** If you have already installed the Data Manager in an earlier version please follow these steps:
  1. install version 1.0 **without** removing the previous version


## Credits ##

Big thanks go to 600WPMPO and Casublett for their great input and help.


## Disclaimer ##
Please note that this script is still beta so you are advised to use it in a testing environment first.

## Donations ##
To help keeping the Data Manager alive and progressing you are kindly invited to donate [here](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=UQ7JZY366R85S)
