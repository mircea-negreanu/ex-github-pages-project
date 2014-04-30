---
layout: page
hero: true
title: Home
show_title: false
---
{% include JB/setup %}


<div class="jumbotron">
  <div class="container">
	<img src="{{ BASE_PATH }}/assets/imgs/logo_flower-platform_big.png" alt="Flower Platform Logo" class="img-responsive center-block"/>
	<p class="text-center" style="color: #666666">Smart<sup>*</sup> <span style="color: #F05A28">mind maps</span> and <span style="color: #F05A28">diagrams</span> for developers</p>
	<small>* <i>smart</i>: see paragraph below for our definition</small>
  </div>
</div>

<h1>What? <small>What is Flower Platform?</small></h1>

Flower Platform is about representing data as **smart mind maps** and **diagrams**. We say that mind maps and diagrams are smart when:

<div><button type="button" class="btn btn-primary btn-xs" data-toggle="collapse" data-target="#what-details">
more ...
</button></div>

<div id="what-details" class="collapse" markdown="1">
1. they show data that comes from **external data sources** (e.g. from source code, development tools, etc.);
1. they allow us (developers) to **interact visually** with the data. And when done, the modifications are synchronized with the original data sources (i.e. 2 way data synchronization);
1. they allow simultaneous **collaboration** between us. **Ubiquity**: access and collaborate on mind maps and diagrams from the web, IDE, mobile.

Flower Platform is **several things**:

* *Flower Platform Core*
  * *Flower Platform Server*: a server application (with a web front-end); it hosts extensions (plugins)
  * *Flower Platform Mobile*: a mobile client for the Flower Platform Server
  * *Flower Platform for IDE*: hosts extensions (plugins) inside popular IDEs
* *Flower Platform Extensions*: plugins that do the actual work
* *Flower Platform Hub*: an online free service: cloud hosted Flower Platform Server and extensions

Flower Platform is **open source**, under GPL v3 license.

</div>

<h1>Why? <small>Why are we developing Flower Platform? Why do we think it's important?</small></h1>

Because of **best practices**:

<div><button type="button" class="btn btn-primary btn-xs" data-toggle="collapse" data-target="#why-details">
more ...
</button></div>

<div id="why-details" class="collapse" markdown="1">
* Best practices recommend us (developers) to use various modern libraries and frameworks. This helps us at **runtime**. 
* Best practices advocate the use of various tools, techniques, development methods, etc. This boosts our productivity by improving our **work flow**.

The state of the art in our field of work (i.e. the number and quality of programming languages, libraries, frameworks, IDEs, development tools, etc.) is **awesome**. But we (the Flower Platform dev team) think that things can be "MOAR" awesome, if we had an intelligent tool that would:

* automatize our work with libs, frameworks, etc. (i.e. the **runtime** area), and
* interconnect some dev tools that we are using (i.e. the **work flow** area).
</div>

<h1>How? <small>Technical overview of Flower Platform</small></h1>

The Flower Platform software ecosystem is composed of:

<div><button type="button" class="btn btn-primary btn-xs" data-toggle="collapse" data-target="#how-details">
more ...
</button>
</div>

<div id="how-details" class="collapse" markdown="1">

### Flower Platform Core

**Flower Platform Core** is a modular platform that makes it easy for extensions to connect to external data sources, represent data visually and to synchronize the data.

**Flower Platform Server** is a server application with a web front-end (i.e. a web app). Sharing and collaboration around mind maps and diagrams are a primary focus. The server side code is written in Java and it's modular, packed as OSGi plugins. The client side code (using Apache Flex and JavaScript) is also modular.

**Flower Platform Mobile** is a mobile client (Android, iOS), that makes it easy for extensions to expose most of their features on mobile,  using **single sourcing** (i.e. same client code runs in the web and mobile environment).

**Flower Platform for IDE** is designed to integrate into IDEs, using an embedded servlet container (Jetty), and an embedded browser. Eclipse is supported natively (being an OSGi container). IDEA is supported as well, using a small Equinox based host wrapper. The same principle can be used to easily support other IDEs in the future. Same **single sourcing** concept applies here as well (i.e. same server and client code runs both in a web deployment or in a IDE/local deployment).

### Flower Platform Extensions

An **extension** is a set of OSGi plugins that do the actual work. I.e. they know how to connect to external data sources, they know how to represent it visually, and they know how to synchronize it. Of course, extensions leverage the convenient API exposed by Flower Platform Core (e.g. diagramming library, data synchronization algorithms, etc.). This way, with **single sourcing**, the same plugin code runs in the web app, the IDE and mobile/tablet.

### Flower Platform Hub

**Flower Platform Hub** is an online free service: the Flower Platform ecosystem, in a cloud based environment. Users have the access to all the features of the Flower Platform & extensions, without having to install and maintain a Flower Platform server. Flower Platform Hub is meant to be used by open source communities.

</div>

<hr>
<div class="page-header">
  <h1>Flower Platform Extensions</h1>
</div>

<div markdown="1">mydiv</div>