# CDN

---

# From [Max Saxe Design Hawk](https://github.com/MaXSaxeDesign/Hawk)

## MaX Saxe Design Hawk is an evolving intelligent bot originally designed for Twitter, now supports Ello, Facebook, Instagram and YouTube

> MaX Saxe Design Hawk supports some of Starbucks integration as of R20.00.00 (December 2015)

> > The idea being MaX Saxe Design Hawk can drive inteligent suggestions of what you should order at Starbucks on multiple social media platforms, it will give you the directions to the nearest Starbucks location & let your friends know you have checked into Starbucks on multiple social media platforms

---

> Currently in development is the [Twitter](https://twitter.com) Intelligent Blocking Bot feature, in R22.00.00

> MaX Saxe Design Hawk will be adding Ghost to the list of supported platforms at some point in 2016

> MaX Saxe Design Hawk will be adding GitHub to the list of supported platforms at some point in 2016

---

> An extension of MaX Saxe Design Hawk will be the ability to interface with [IFTTT](https://ifttt.com) to link in with IFTTT recipes

> > MaX Saxe Design cannot confirm when [IFTTT](https://ifttt.com) will be a supported feature

---

## Hosting

Hawk is currently hosted on local MaX Saxe Design servers and in the London and San Francisco [Digital Ocean](https://digitalocean.com) Data Centres.

Hawk can be put into production anywhere on the Digital Ocean network due to [MaX (CET & Founder of MSD)](https://twitter.com/MaX_MSD) making builds in every single Digital Ocean data centre to take snapshots to enable Hawk to stay online whatever the state of the Digital Ocean data centre networks or more allarmingly, the Internet.

## MaX Saxe Design takes data and network security very seriously and prides itself on highly available and secure systems.

The passwords used to log into the Hawk system are stored in hardened systems with only internal networking with no external connections.

## The route to the servers is a little different to standard CDNs and hosting networks

> There are a few types of servers:

> > Cache server

> > Cache request server

> > Origin server

> > Origin request server

> > Edge server

> > > Edge authorisation server

> > > Edge request server

> > Edge password server

> > Core server

> > > Core authorisation server

> > > Core request server

> > Core database server

> > Core password server

> > Core SAN

> > Production push server

> > > Allows MaX Saxe Design to autonomously upload to the server network

## Requesting Data and Passwords

#### Cache Server

> The user request hits the cache server

> > If a password is requested it hits the cache request server

> > > The cache request server hits the edge password server

> The cache server requests an update every ten seconds from the origin server

#### Origin Server

> The cache server hits the origin server

> > If a password is requested it hits the origin request server

> > > The origin request server hits the edge password server

> The origin server requests an update every twenty seconds from the edge servers

#### Edge Server

> The origin server hits the core server

> > If a password is requested it hits the edge password server

> > > The internal request server hits the edge password server

> The edge servers request an update every thirty seconds from the core servers

> The edge server authorises the connectivity to the edge password server

#### Core Server

> The core server authorises the connectivity to the core password server

> > The only server able to connect to the core password server is the edge password server for updates - triggered by the and update on either password server

#### Production Pusher Server

> The production pusher server autonomously uploads to the core server and the rest of the CDN when updates need to be made

> There are equivelents for the database and SAN sub network sectors of the CDN

## [MaX](https://twitter.com/MaX_MSD) is to blame for the password servers request servers:

> The password servers in question run on custom systems and do not give the password back to the server

> The password servers are stores and cannot release any information

> These stores compare the multi-layered encrypted information and provide an authorisation key, which changes every second

---
