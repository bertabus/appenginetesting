appenginetesting
===============

Fork of [gae-go-testing](https://github.com/tenntenn/gae-go-testing) with a few minor changes:
- renamed for nicer import syntax (that IDEA's Go Plugin won't highlight as an error)
- added +build tags so that it compiles
- simplified install instructions. 

    * GAE/G 1.7.0, go 1.0.3
    * GAE/G 1.7.1, go 1.0.3

Installation
------------

Set environment variables :

    $ export APPENGINE_SDK=/path/to/google_appengine
    $ export PATH=$PATH:$APPENGINE_SDK

Before installing this library, you have to install
[appengine SDK](https://developers.google.com/appengine/downloads#Google_App_Engine_SDK_for_Go).
And copy appengine, appengine_internal and goprotobuf as followings :

    $ export APPENGINE_SDK=/path/to/google_appengine
    $ ln -s $APPENGINE_SDK/goroot/src/pkg/appengine
    $ ln -s $APPENGINE_SDK/goroot/src/pkg/appengine_internal


This library can be installed as following :

    $ go get github.com/icub3d/appenginetesting


Usage
-----

The
(documentation)[http://godoc.org/github.com/icub3d/appenginetesting]
has some basic examples.  You can also find complete test examples
within [gorca](https://github.com/icub3d/gorca)/(*_test.go). Finally,
[context_test.go](https://github.com/icub3d/appenginetesting/blob/master/context_test.go)
and
[recorder_test.go](https://github.com/icub3d/appenginetesting/blob/master/recorder_test.go)
show an example of usage.
