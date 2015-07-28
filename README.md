# coffee-node-skeleton
set yourself up right

Install Xcode:
Open and agree to terms

Install Homebrew:

ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”

Download SublimeText 3:

http://c758482.r82.cf2.rackcdn.com/Sublime%20Text%20Build%203083.dmg

<strong>Install Sublime Package Control:</strong>

ctrl+`

Type into python console:

import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)


Install Better Coffeescript:

cmd+shift P

Package Control:

Install Package

“Better Coffeescript”

Install Jade:
cmd+shift P
Package Control: Install Package
“Jade"

Install npm:
brew install npm

Install mongodb:
brew install mongodb
sudo mkdir /data
sudo mkdir /data/db
sudo chown -R `id -u` /data/db
Install nodemon:
npm install -g nodemon

Set up skeleton:
git clone this repository
npm install in repo directory
Terminal Tabs: mongod, nodemon app.coffee

Testing:
mongo
- show dbs
- "use project" (use the database name “project”)
- "show collections" (collections of data within database)
- "db.users.find()" (find all users in the database)
postman
- in chrome: https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en
view content in browser
- http://localhost:3005 (assuming PORT is 3005)
