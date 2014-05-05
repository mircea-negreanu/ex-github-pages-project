---
layout: page
group: subconcept
parent-id: core

title: "File System"
labels: [implemented, in-progress]
#tagline: "tagline"
comments: true
share: true
# in case you want to force a disqus identifier, when you rename the page
# get the disqus identifier from the original page (something like var disqus_identifier = 'ident';),
# uncomment the following line and replace the text between "" with ident
#comments_identifier: "identifier"
---

{% include JB/setup %}

## TODO: write about file system

## Download

When you have finished working with your code on Flower Platform and you're ready to export it back to your local file system, go to the file/directory you wish to download and choose the **Download** action. 

<img class="img-thumbnail center-block" src="download.png"/>

The contents of a directory will be placed in a ``.zip`` file.

The file will be downloaded using your browser's download manager. 

<div class="alert alert-info">
Although Flash Player has no restriction on the size of files you can upload or download, the player officially supports uploads or downloads of up to 100 MB.
</div>

## Upload

To upload files from your local file system into Flower Platform, use the **Upload** action.

<p class="text-center">
<img class="img-thumbnail" src="upload1.png"/>
<img class="img-thumbnail" src="upload2.png" hspace="20"/>
</p>

Only single files are supported. 
To upload multiple files, store them in a ``.zip`` file. Flower Platform will ask you if you want to unzip it.

<img class="img-thumbnail center-block" src="upload3.png"/>