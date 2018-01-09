# poly-on-fire-roles-DB-permissions
Barely useful code that I use as a baseline for keeping role based permissions logical in my own head, especially compared to UI visibility

This readme is to be fleshed out later.

# most code removed

There is only one relevant file in this repo - database.rules.json

# motive

This project is a companion to poly-on-fire-roles-UI-visibility and exists to stress the point that the developer must implement role based security on two entirely separate systems - UI and DB - and coordinated manually, at the code level.

* The UI can be hijacked at any time, such as in chrome dev tools, and make visible any portions that the developer intended to keep from prying eyes by role, such as making admin views visible to anyone.
* The DB would probably have the same roles and protections as the UI, except on the DB it can't be hijacked :) So you can make the admin view visible, it just won't show any records unless you have the proper permissions on the DB side.

# Reference

See https://angularfirebase.com/lessons/understanding-firebase-database-rules-by-example/ for source of this code
