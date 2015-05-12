---
layout: post
title:  "SSH login without password"
date:   2015-05-12 16:00:00
---

Why? Because SSH-ing anywhere that involves you typing your password isn't secure, and that means you've to remember or write down the password somewhere, totally stone-age method.

Here's what you need to be able to SSH without password from your computer (`client`) to somewhere else (`host`):

* Credentials to `SSH` into the `host` server.
* A public key. Here's [how you can generate it](https://help.github.com/articles/generating-ssh-keys/).
* Ability to follow instructions.

Once you have all of the above, let's go:

* Login to the `host` via `SSH` (one time only, I swear!)
* Navigate to `~/.ssh` directory on `host`, if it does not exist create it. It should have `700` permission (`chmod 700 ~/.ssh`)
* If it doesn't exist already, create `~/.ssh/authorized_keys` file with `600` permission.
* Append your public key (usually located in `~/.ssh/id_rsa.pub` on your computer) in `host`'s `~/.ssh/authorized_keys` file.
* Profit.
