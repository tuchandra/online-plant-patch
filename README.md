# cc-harvest
Adds a link to users' plant patches on the Click Critters Users Online page, for the Haunted Harvest event.

## Overview
![ClickCritters users online page](/images/online.PNG?raw=true)

[Click Critters](https://www.clickcritters.com) is a virtual adoptable site where users can collect adoptables and play many games. During an event running in December 2016, called Haunted Harvest, users are encouraged to visit other users' "plant patches." These contain plants that one can interact with ("click"). In exchange, other users will click your own plants.

This event lends itself to users visiting the patches of other users who are online. While Click Critters has a page listing online users, an additional click is required from this page to reach a user's plant patch (one must navigate to their profile page).

This extension removes that need. By tweaking the users online page, this facilitates participation in the event by making it easier for people to reach others' plant patches.

## Maintenance
Users' profile pages, which are linked on the users online page, are created with usernames. Their plant patch pages are created with their userIDs. While the mapping from usernames to userIDs is one-to-one (each username has a unique userID), this mapping is not publicly available.

A manual map of username : userID pairs must therefore be kept. The extension only adds links for users whose usernames are contained in userids.js (otherwise, it has no way of determining the userID). Therefore, userids.js must be updated periodically.