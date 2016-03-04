# booc
After several months of trying every OSX related setup/install/configuration management approach known to man, I think this is (for me, for now) finally the one. Ansible is a tool I use each day at HP Enterprise, and I like it more and more as I use it. Puppet, Chef, bash, python, etc. are all fine tools for their many uses. This is the approach that has FINALLY felt right for me.

1. Lightweight - just enough Ansible to get the job done
2. Simple - most of what I need in one git repo
3. Personal - not a fork of someone else's repo, but all of it my own

Here's to bringing order out of the chaos of managing a modern development workstation.

# Preparation
1. Install 1Password from the Apple Store; sync with iCloud.

2. Install SSH keys from 1Password.
  - copy files from 1Password to ~/.ssh
  - chmod 700 ~/.ssh/id_rsa

3. Accept the XCode license agreement
```
git status
```

4. Clone this repo locally & cd into the repo folder
```
git clone git@github.com:wchrisjohnson/booc.git ~/.booc
cd ~/.booc
```

# Let's do this!
```
./install <machine-name>.yml
```

# Restore configs for selected apps
```
mackup -v restore
```

# Apps that require manual install
Currently, installing OSX applications that have a GUI is a bit problematic. Granted I'm a bit OCD, but I've had issues beyond just aesthetics with linking apps into the ~/Applications folder. So for now, I'm not gonna do it.

Two possible solutions:

1. If the brew-cask team gets their stuff working by MOVING apps into the ~/Applications folder
2. If I discover an Ansible based approach for cleanly installing apps.

For now, this is just my todo list.

* Blue Jeans
* Dash 3 (App Store)
* Flux
* Google Chrome
* Google Drive
* GPG Keychain
* Handbrake
* HipChat
* HP MyRoom
* istat-menus4
* Junos Pulse
* Marked (App Store)
* Microsoft Lync
* Microsoft Office 2016
* Microsoft OneNote (App Store)
* Microsoft OneDrive (App Store)
* NetSpot
* P4Merge
* Pycharm 5
* Screenhero
* Skitch (App Store)
* Skype
* Space Gremlin Pro (App Store)
* SuperDuper!
* TextMate 2
* Textual 5 (App Store)
* Tower 2
* TunnelBlick
* Tweetbot (App Store)
* vagrant
* VMware Fusion 7

* Docker Toolbox
* Microsoft Studio Code
