---
layout: post
title: Debian VPS setup
category: linux
---

Set a strong root password
'passwd'

Run updates
'apt-get update && apt-get upgrade'

Install your favorite editor, I like nano.
'apt-get install sudo nano'

Make your preferred editor the default
'sudo update-alternatives --config editor'

Create a non-root user for general system operations
'adduser sysop'

Add the new user to the sudoer group
'adduser sysop sudo'

Switch users
'su sysop'

install the apache2 package

'sudo apt-get install apache2 -y'

Coming soon: updating the default Apache configuration.