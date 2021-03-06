Notify.io
===
Notify.io is the open notification platform for the web. 

These notes are for people that are interested in contributing or learning about about Notify.io works. If you just want to use it to get notifications, sign up at [Notify.io](http://notify.io).

Getting Started
---
You need the [Python App Engine SDK](http://code.google.com/appengine/downloads.html#Google_App_Engine_SDK_for_Python) installed. To start the server

    dev_appserver.py -p 8081 www

If your shell can't find the `dev_appserver.py` command, you need to [create a symlink to this command](http://code.google.com/appengine/docs/python/gettingstarted/devenvironment.html).

Alternatively, if you don't want to use the shell you can use the App Engine Launcher.

**Note**: When running in development mode, these outlets will not work:

* Desktop Notifier
* Email (unless you [set it up](http://code.google.com/appengine/docs/python/tools/devserver.html#Using_Mail))
* any outlet that requires keys

Running tests
---
You'll need these packages:

* [nose](http://somethingaboutorange.com/mrl/projects/nose/1.0.0/)
* [NoseGAE](http://farmdev.com/projects/nosegae/)
* [WebTest](http://pythonpaste.org/webtest/)

Run the test suite with:

    nosetests --with-gae

or edit your .noserc accordingly. Make sure you're in the www directory.

