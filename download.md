---
layout: page
title: "Download"
comments: true
---

{% include JB/setup %}

# Flower Platform Web App

<p><a class="btn btn-success" href="#">Download Flower Platform Web App<br>v0.1.0 (Proof of Concept)</a></p>

## Install / Upgrade

### Install Tomcat <small>(skip if Tomcat is already installed)</small>

Flower Platform Web App runs inside the [Apache Tomcat](http://tomcat.apache.org/) server. Please install it on your system. If this is something new to you, please use Google to find out more. There are plenty of tutorials (written and video).

We work with Tomcat v7; we haven't tested it with v8, but we don't see any reasons why it shouldn't work.

### Remove Older Version of Flower Platform <small>(skip for first installation)</small>

Stop Tomcat. Go to the ``TOMCAT_INSTALL_DIR/webapps`` directory of your Tomcat installation. Remove:

* ``flower-platform.war`` file and
* ``flower-platform`` directory

<div markdown="1" class="alert alert-info">
**Remark regarding the data (workspace) directory.** By default Flower Platform stores its data in ``TOMCAT_INSTALL_DIR`` (cf. ``TOMCAT_INSTALL_DIR/webapps/flower-platform/WEB-INF/web.xml`` -> search for *workspaceLocation*). 

So if you didn't change this default setting, your data is safe when you delete the dir + file, cf. above. Otherwise, if you did change this setting and you configured the location within the webapp itself, then be careful when you delete the webapp directory.
</div>

<div markdown="1" class="alert alert-warning">
We'll improve the update procedure in the future, by using the Eclipse Update Site mechanism + Eclipse P2.
</div>

### Copy the .war File

* Make sure that Tomcat is stopped. 
* Copy ``flower-platform.war`` -> ``TOMCAT_INSTALL_DIR/webapps/flower-platform.war``
* Start Tomcat. After the server has started, you should see a ``flower-platform`` directory (i.e. the unpacked contents of the ``flower-platform.war`` archive file).

<p markdown="1" class="text-success">Flower Platform should now be accessible from your web browser. Usually at [http://localhost:8080/flower-platform](http://localhost:8080/flower-platform).</p>

<div markdown="1" class="alert alert-info">
If you encounter **difficulties** in installing Flower Platform, please **start a discussion** below.
</div>

# Flower Platform Mobile

Flower Platform Mobile can be installed on Android devices from Google Play [here](#).

# Flower Platform for IDE

We'll make it available as soon as IDE enabled extensions will be released. 
