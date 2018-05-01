*poly-on-fire* is a collection of proof-of-concept projects using [Polymer](https://www.polymer-project.org/) and [Firebase](https://firebase.google.com/)

|[**_Pete Carapetyan_**](http://appwriter.com)|  [TL;DR? blog](https://betterologist.net/2018/04/poly-on-fire-polymer-on-firebase/) |[TL;DR? _video:_](https://youtu.be/P9DwkqqUxNs)|
| --- | --- | --- |
|<a href="http://appwriter.com"><img class="style-svg" src="https://betterologist.net/wp-content/uploads/2016/05/pete-300x297.jpg" alt="pete" width="116" height="115" /></a>|<a href="https://betterologist.net/2018/04/poly-on-fire-polymer-on-firebase/" ><img class="style-svg" src="http://docs.datafundamentals.com/txt.png" alt="jammazwanPhotoSmall" width="200" height="116" /></a>|<a href="https://youtu.be/P9DwkqqUxNs"><img class="style-svg" src="https://betterologist.net/wp-content/uploads/2016/05/jamzVid1.png" alt="about" width="115" height="115" /></a>|


##### A project for learning an aspect of developing a Polymer app, deployed on Firebase hosting.

The idea is to prove out an approach or component in the simplest project first, before combining it with other code in a real project.

----

# \<poly-on-fire-roles-DB-permissions\>

# PROJECT IRRELEVANT BECAUSE:

Since writing this project I discovered JWT Custom Claims from this video
https://youtu.be/JOASK1BL67M

I will be implementing that at some future date, probably in Polymer3

## What it does:

Barely useful code that I use as a baseline for keeping role based permissions logical in my own head, especially compared to UI visibility

# most code removed

There is only one relevant file in this repo - database.rules.json

# motive

This project is a companion to poly-on-fire-roles-UI-visibility and exists to stress the point that the developer must implement role based security on two entirely separate systems - UI and DB - and coordinated manually, at the code level.

* The UI can be hijacked at any time, such as in chrome dev tools, and make visible any portions that the developer intended to keep from prying eyes by role, such as making admin views visible to anyone.
* The DB would probably have the same roles and protections as the UI, except on the DB it can't be hijacked :) So you can make the admin view visible, it just won't show any records unless you have the proper permissions on the DB side.

# Reference

See https://angularfirebase.com/lessons/understanding-firebase-database-rules-by-example/ for source of this code
