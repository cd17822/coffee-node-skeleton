# coffee-node-skeleton
set yourself up right

<strong>Install Xcode:</strong></br>
Open and agree to terms

<strong>Install Homebrew:</strong></br>
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”

<strong>Download SublimeText 3:</strong></br>
http://c758482.r82.cf2.rackcdn.com/Sublime%20Text%20Build%203083.dmg

<strong>Install Sublime Package Control:</strong></br>
ctrl+`<br>
Type into python console:<br>
```python
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

<strong>Install Better Coffeescript:</strong></br>
cmd+shift P<br>
Package Control:<br>
Install Package
“Better Coffeescript”

<strong>Install Jade:</strong></br>
cmd+shift P
Package Control: Install Package
“Jade"

<strong>Install npm:</strong></br>
brew install npm

<strong>Install mongodb:</strong></br>
brew install mongodb
sudo mkdir /data
sudo mkdir /data/db
sudo chown -R `id -u` /data/db
Install nodemon:
npm install -g nodemon

<strong>Set up skeleton:</strong></br>
git clone this repository
npm install in repo directory
Terminal Tabs: mongod, nodemon app.coffee

<strong>Testing:</strong></br>
mongo
- show dbs
- "use project" (use the database name “project”)
- "show collections" (collections of data within database)
- "db.users.find()" (find all users in the database)

postman
- in chrome: https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en

view content in browser
- http://localhost:3005 (assuming PORT is 3005)
