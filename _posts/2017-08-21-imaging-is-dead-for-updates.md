---
layout: post
title: Imaging Is Dead… for Upgrades
---
I go on vacation and what happens? Apple decides it's time to answer some of the Mac Admin community's burning questions. Let's queue up the articles, shall we?

- [Prepare your institution for iOS 11, macOS High Sierra, or macOS Server 5.4](https://support.apple.com/kb/HT207828)
- [Prepare for APFS in macOS High Sierra](https://support.apple.com/kb/HT208018)
- [Prepare for changes to kernel extensions in macOS High Sierra](https://support.apple.com/kb/HT208019)
- [Upgrade macOS on a Mac at your institution](https://support.apple.com/kb/HT208020)
- [Prepare for changes to Content Caching in macOS High Sierra](https://support.apple.com/kb/HT208025)

The KBase article I want to address in this blog post is that fourth one, "Upgrade macOS on a Mac at your institution."

Apple has now stated directly what a lot of people in the community have been suggesting: Imaging, as a method
of deploying new/upgraded operating systems, is dead as far as Apple is concerned. It's officially unsupported.
"Apple doesn't recommend or support monolithic system imaging when upgrading or updating macOS." Can't get much more explicit than that.

Contrary to some earlier predictions, Apple does not appear to be eliminating access to all forms of imaging. In the article, they explicitly
state, "You can use system images to re-install the existing operating system on a Mac." That led some to believe that if they
used one of those cumbersome methods I mentioned in my [previous blog post](/2017/08/12/firmware-follow-up.html) to put firmware updates into place,
they could continue to (capture and) deploy images; Everything is Fine _(insert meme reference here)_.
That is not the approach I am taking. 

The main reason I believe imaging hasn't gone away completely yet is because Apple needs a tool like that to use at the factory. If there's one
place where efficiency and speed is King, it's in initial production. Whether Apple always chooses to make that tool
accessible to Mac Admins is another discussion (especially when APFS becomes more mature and feature-rich), but Apple has identified at least one
imaging use case (perhaps handing an old computer to a new student/employee/user) where they don't currently have a good alternative in place, so they have continued to make imaging available.
Keeping that in mind, I'm willing to take Apple at its word; I should stop jumping OSes using an image as a base. I've been thinning my [modularly-created image](https://github.com/magervalp/autodmg)
every year such that I'm in good shape to eliminate imaging by this time next year (my next major planned redeployment).

People in the community have been saying "imaging is dead" for a couple of years now (even longer for capturing monolithic images).
Now Apple has weighed in. Ignore their direction at your professional peril.
