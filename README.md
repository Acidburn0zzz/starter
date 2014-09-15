hi!
===

![ninjabong](ninjastar.jpg "ninjabong")

my [osxc](http://osxc.github.io) playbook, already forked ! (and in-progress porting from legacy-osxc)


> **Warning:** This version of [osxc](http://osxc.github.io) is not compatible with the old one (called now legacy), you'll have to copy some old roles locally in order to make a smooth transition. On the other side, you can still use legacy and we will continue to accept your pull requests on legacy.

## Introduction

Welcome to [osxc](http://osxc.github.io) !

[osxc](http://osxc.github.io) is a simple configuration tool for OS X (in fact, it just makes it easier for you to use ansible on OS X).

You can reach our (temporarily not updated and old) [website](http://osxc.github.io) if you want to know more. But don't follow the instructions there to get started, just stay here for that !

## Getting started

> **Warning:** All of this is subject to change, just be sure you're able to reach this page to see the latest instructions when it'll be updated. Don't worry though, we will not change brutally the structure of your current repo (not like we did with legacy). All we are going to do is add a CLI tool.

> **Additional Note:** If you're installing system-wide `sudo ansible-galaxy install -r requirements.yml` otherwise edit `ansible.cfg` and uncomment `#roles_path:./roles` to install the roles in your osxc/starter fork before running **Step 5**

1. Be sure to have the XCode Command-Line tools installed: `xcode-select --install`
2. Manually install Ansible 1.8 with ``git clone https://github.com/ansible/ansible.git ~/src/github.com/ansible/ansible; cd ~/src/github.com/ansible/ansible; sudo make install``
3. While that's happening [Fork this repo](https://github.com/osxc/starter/fork) and then clone your fork anywhere you want on your machine: `git clone git@github.com:<myname>/starter.git; mv starter osxc; cd osxc`
4. Take a quick look at `configuarion.yml` and `installation.yml` customizing to your liking.
5. Start osxc with `ansible-galaxy install -r requirements.yml && ansible-playbook desktop.yml`

At the end, you'll only need to repeat step 5.

Now you're ready to further tweak the configuration we gave you. Have fun ! (You may want to read the [Ansible documentation](http://docs.ansible.com/index.html) in this case ...)

## Learn More

If you want to get more documentation or just want to see what [osxc](http://osxc.github.io) can do for you, here's a [repository list on ansible galaxy](https://galaxy.ansible.com/list#/users/6499) where you can find all the publicly available roles for [osxc](http://osxc.github.io).
