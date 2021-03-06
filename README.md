# clients-and-profits-greaser
A Greasemonkey / Tampermonkey userscript for making the C+P web interface a little more tolerable.

## About
This userscript uses mutation observers to make some subtle interface changes to the C+P web interface.  Currently this script will:

1. Crush a few annoying alert messages about missing budget hours.
2. Force capitalization of job numbers and task codes in the timesheet form.

## Installation
Installation should be handled via a URL installer and not copied/pasted.  This will allow your application to receive updates when available.  In Tampermonkey you can use the "Install from URL" feature available in teh Utilities menu.  The URL to install is this...

`https://raw.githubusercontent.com/treetop1500/clients-and-profits-greaser/master/tamper.js`

## Updates
When script updates are available you can tap on the 'Last updated' value of this script in the Installed Userscripts menu of the Tampermonkey interface and it will update to the most recent version on Github.

## Configuration
You'll need to configure the script to run on the correct domain.  For security purposes, I won't post the domain in this readme, but surely you can figure that out.  It's the URL you go to when you use C+P.  In Tampermonkey it will be in the Includes/Excludes section of the settings under "Original Matches".  The value will look like https://XXXXXXX.jobr.mobi/index.php

## Contributing
Another annoying message you'd like to squash? Want to get one with your inner hacker? If you'd like to help make improvements feel free to fork this project and send pull requests!

## To Do
 - Make string comparisons on alert messages lowercase to future proof any changes in case that may occur in updates.
 - Track down the auto complete problem where job numbers on timesheet entries can double up if you type to fast.  This may have to do with the CSS fade animation on that control.
