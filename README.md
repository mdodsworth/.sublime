# Settings for Sublime 2

## Installation

- clone this repository into your home directory
- run Sublime at least once so that the its config/settings directories are created
- remove the generated `User` config directory
	
	rm -rf ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/User

- create a symbolic link to the cloned `User` directory

	ln -s ~/.sublime/User ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/User

- install wbond's Sublime package manager through the Sublime console (accessed via `ctrl+\``)

	`import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'`
