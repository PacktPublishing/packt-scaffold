# Platform Availability

Another short section (who has time to write pages and pages of documentation?). The application container we're using is based on [Electron](http://electron.atom.io). This lets us wrap a modified GitBook project around a set of cross-platform outputs. That's all this is. It's relatively quick to setup a new project, and we can definitely turn it into a process :).

Out of the box, Elextron supports:

* Windows (including the new Windows 10 format for the Windows Store)
* OSX (so .dmg, and we can also sign the applications if we want to sell those on the App Store)
* Linux

Deploying to application stores is the sort of thing thats a little more involved (certificate signing and filling in a bunch of online forms), but it's possible as we're effectively building native applications. This is also a last-resort for being able to list courses and video products on Amazon, as part of the software store.
