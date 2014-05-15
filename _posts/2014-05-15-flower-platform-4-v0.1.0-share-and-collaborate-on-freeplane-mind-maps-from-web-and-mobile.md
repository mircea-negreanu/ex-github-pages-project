---
layout: post
title: "Flower Platform 4 v0.1.0 Released. Share and Collaborate on Freeplane Mind Maps. From web and mobile"
tags: [news, releases]
---

After many months of hard work, the Flower Platform team is very proud to announce the release of:

* **Flower Platform 4** v0.1.0: Core and Mind Map Extension - The very first public version, which is a *proof of concept* version. It's far from being stable, but it illustrates what the platform is capable of.
* **Flower Platform Hub**, available at [http://hub.flower-platform.com](http://hub.flower-platform.com) - Take a look at Flower Platform 4 online, without installing the server on your computer.
* **The new web site** - Flower Platform 4 is different from its predecessors both conceptually and technically. We have updated the content of the web site to reflect the specifics of Flower Platform 4. Take a look at the [home page](/) to learn more about Flower Platform 4.

<span class="label label-primary">Guide!</span> We have prepared a small guide that would help you make a quick tour of Flower Platform. More precisely:

From the web browser:

* manage files
* upload/download files (and Freeplane mind maps)
* work and collaborate with other people on Freeplane mind maps

And then use Flower Platform Mobile for Android.

<!-- more -->

<img class="img-thumbnail center-block pull-right" src="/blog-img/2014-05-15/flow-main.png"/>

<div markdown="1" class="clearfix">

# Flower Platform Web App

<span class="badge">1</span> **Go to** <a href="http://hub.flower-platform.com/" target="_blank">Flower Platform Hub</a>. You can also [download and install](/download.html) Flower Platform on your system, but for a quick start, we recommend Flower Platform Hub.

The first thing you'll notice should be the ``root`` editor that is already open when the application is loaded. There is a ``repository`` node (containing data about the existing repository on the server) and a ``_debug`` node (containing technical data, e.g. active sessions, open resources, etc.).

<span class="badge">2</span> **Navigate** to the ``repository/fileSystem`` node. It lists directories and files on the file system.

<span class="badge">3</span> **Create a directory** (e.g. myFirstName-myLastName): right-click on the ``fileSystem`` node and choose **New File/Folder**. This will be your playground.

<span class="label label-success">Tip:</span> More details on working with the file system are available in [the file system section](/concepts/core/#FileSystem).

### Upload your mind maps

<span class="badge">1</span> You can **upload** an existing mind map file from your local file system to Flower Platform's file system, using the **Upload** action on your directory. The file will appear as a child node of the directory node, and can be opened right away.

<p class="text-center">
<img class="img-thumbnail" src="/blog-img/2014-05-15/flow-upload1.png"/>
<img class="img-thumbnail" src="/blog-img/2014-05-15/flow-upload2.png"  hspace="10"/>
</p>

<img class="img-thumbnail center-block" src="/blog-img/2014-05-15/flow-upload3.png"/>

<span class="badge">2</span> Of course, you can also **create a new mind map** from scratch, using the **New File/Folder** action. Make sure to append the ``.mm`` extension; this way the file will be processed as a mind map and opened in the corresponding editor.

<span class="badge">3</span> Now that you have a mind map, you can **view** it, **edit** nodes and **save** your work, almost as if you were working with the Freeplane desktop application.

<span class="label label-success">Tip:</span> To see what's available for the mind map editor, visit [the mind map section](/concepts/mind-map). We are working on supporting more and more features from Freeplane. Working with editors in general is detailed in [the editor section](/concepts/core/#Editor).
</div>

### Share your mind maps

You can easily share your work with others; any modification you make on your mind map will be automatically propagated to any other user who has the file open in an editor.

To invite others to a collaborative work session on one (or more!) of your mind maps, go to the **Navigate > Get/Follow Link** action in the global menu. We provide a link to the currently active editor, as well as to all the editors you have open.

<img class="img-thumbnail center-block" src="/blog-img/2014-05-15/flow-link.png"/>

The link may be pasted in the browser's address bar. In this case the editor(s) will be opened as soon as the application is loaded. If you already have the FP Hub open in your browser, you can also paste the link the **Follow** text input in the **Get/Follow Link** dialog to open the editors in the same application.

<a href="flow-collab-big.png">
<img class="img-thumbnail center-block" src="/blog-img/2014-05-15/flow-collab-small.png"/>
</a>

### Download your mind maps

After saving your files, you may download them with the **Download** action in the context menu. Download individual files, or your entire directory, in which case the contents of the directory will be packed as a ``.zip`` file.

# Mobile Application

Download the mobile application from the Google Play Store: LINK ???

The app is automatically configured to connect to the Flower Platform Hub. [The mobile section](/concepts/mobile/#ServerAccountsscreen) details the server accounts management.

<img class="img-thumbnail center-block" src="/blog-img/2014-05-15/flow-mobile-config.png"/>

Same as with the desktop application, the ``root`` editor is already opened. Navigate to the ``fileSystem`` node and set up your playground as recommended above, or go to an existing directory. On the mobile app, global and contextual actions can be run from the menu button.

Since the mobile application was specifically designed as a quick way to view and edit mind maps when you don't have access to your desktop computer or laptop, downloading and uploading files is not available. Existing mind maps can be opened, edited and saved, and new mind maps may be created.

You may open as many editors as you'd like. To switch between editors or close an editor, tap the **Editors** button. This will display a callout component that contains the opened editors.

<img class="img-thumbnail center-block" src="/blog-img/2014-05-15/flow-mobile.png"/>

</div>