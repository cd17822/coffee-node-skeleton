# coffee-node-skeleton
## Set yourself up right.
<br>

### Set Up

Clone repository: `git clone https://github.com/cd17822/coffee-node-skeleton.git`

Change into repo directory: `cd coffee-node-skeleton`

Install modules: `npm install`

Terminal should be running (each its own window): `mongod` `nodemon app.coffee`

Not working? See below if there are additional configurations you've yet to set up.

### The Basics

**Install Xcode:**<br>
Open and Agree to Terms

**Install Homebrew:**</br>
`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)”`

**Install npm:**</br>
`brew install npm`

**Install mongodb:**</br>
`brew install mongodb`<br>
`sudo mkdir /data`<br>
`sudo mkdir /data/db`<br>
```sudo chown -R `id -u` /data/db```

**Install coffee-script:**<br>
`npm install -g coffee-script`

**Install nodemon:**<br>
`npm install -g nodemon`

### Editing

**Download SublimeText 3:**</br>
<http://c758482.r82.cf2.rackcdn.com/Sublime%20Text%20Build%203083.dmg>

**Install Sublime Package Control:**

Open Python Console: **ctrl+`**

Type into python console:<br>
```python
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

**Install Better Coffeescript:**</br>
cmd+shift+P<br>
_Package Control: Install Package_<br>
_Better Coffeescript_<br>

**Install Jade:**</br>
cmd+shift+P<br>
_Package Control: Install Package_<br>
_Jade_<br>



###Testing

**View content in browser**<br>
Assuming port is 3005: <http://localhost:3005>

**Use Postman to test API Calls**<br>
Download in chrome: <https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en>

**Sift through MongoDB**

- Begin mongo shell: `mongo`
- Show databases in your system: `show dbs`
- Use database "project": `use project`
- Show collections in project `show collections`
- Find all users in current database: `db.users.find()`
