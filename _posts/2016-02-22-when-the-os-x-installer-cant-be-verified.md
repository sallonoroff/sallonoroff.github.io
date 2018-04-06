---
id: 1980
title: 'When the OS X Installer can&#8217;t be verified.'
date: 2016-02-22 13:22:44 +00:00
author: mark
layout: post
tags:
  - apple
  - fix
  - hints
  - mac
  - osx
  - installer
---
So you've got an OS X installer app saved (or maybe you've [followed some instructions and made yourself a bootable USB drive for installing Mac OS X](http://www.sallonoroff.co.uk/blog/2015/11/make-a-bootable-usb-drive-with-createinstallmedia/)), used it a few times without any issue, forgotten about it, then some time later tried to use it again and run into an error message like this...

> This copy of the Install OS X El Capitan application can't be verified. It may have been corrupted or tampered with during downloading.

(Obviously "El Capitan" here could just as easily be the name of any of the versions of OS X that have been released via the Mac App Store - Lion, Mountain Lion, Mavericks, Yosemite or El Capitan.)

...and now you're wondering what's going on?

You'll quickly find lots of [helpful](http://blog.mconserv.net/2013/10/install-os-x-mavericks-application-cant.html) [stuff](https://thefastforwarding.wordpress.com/2015/10/09/how-to-fix-this-copy-of-the-install-os-x-el-capitan-application-cant-be-verified/) [online](http://www.needhelp4mac.com/2014/10/this-copy-of-the-install-os-x-yosemite-application-cant-be-verified-it-may-have-been-corrupted-or-tampered-with-during-downloading/) suggesting that this problem can be rectified by changing your Mac's system date[^fn-1date]. And, as far as I can tell, that's exactly right. That does work. But some people have success with setting the clock to the current date, while others report that the system date already is correct and they're having to set it to a date in the past to get anywhere. Well, after lots of scouring, here's the best explanation I've found, [buried in the middle the comments section of an OSXdaily.com article](http://osxdaily.com/2015/01/19/fix-os-x-install-errors-cant-be-verified-error-occurred-preparing-mac/#comment-1615940):

> [...] the reason why you get the error (and it’s not because it’s “buggy”) is because the installer app is digitally signed with a certificate (along with every other Mac App Store app, and others app you might download), every certificate has two immutable dates built into it, a “not valid until” (Start) date, and a “valid until” (End) date.
> 
> When you run an app, it verifies the digital signature/certificate, and part of this validation is checking the date bounds, if your computer is set to an invalid date such as 1984… It’s going to fail to verify the certificate.

Right, so thanks to Russell, we now know there's actually a window of validity on these installers. So if you're saving them outside the Applications folder (so that they don't get auto-deleted after use) or making bootable USB drives with them, you're probably going to need to download fresh copies from the App Store when required, or temporarily set your system date to a point approximately around the time you originally downloaded it. You did make a note of that, right?

<span style="color: #999999;">...</span>

**Update:** I stumbled across [this page which says the certificate used to sign Mac App Store downloads expired on 15th February 2016](https://derflounder.wordpress.com/2016/02/15/certificate-expiration-and-downloaded-mac-app-store-installers/). This coincides perfectly with my own problems. So, if you don't want to mess about temporarily altering your Mac's date when you need to install, go download fresh copies from the MAS (now signed until 7th February 2023).

Oh, but if you do want/need to check the certificate start/end dates of an installer you already have saved, throw this command into Terminal and scan the resulting output:

`openssl pkcs7 -inform der -in /Applications/Install\ OS\ X\ Mavericks.app/Contents/_MASReceipt/receipt -print_certs -text`

(This example checks the Mavericks installer in the Applications folder. Adjust the path accordingly for your own needs.)

[^fn-1date]: You can change the date via System Preferences if you still have a working OS X installation aboard the Mac, or by using the '[date](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/date.1.html)' command in Terminal if you're having to boot from a createinstallmedia-made USB drive.
