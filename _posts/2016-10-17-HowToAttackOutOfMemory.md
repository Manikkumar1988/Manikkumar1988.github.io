---
layout: post
title:  "How to Attack OOM"
date:   2016-10-17 23:25:49
customjs:
 - https://gist.github.com/Manikkumar1988/bd9f058084d56885d1bdae3bdd309649.js
---

## How to Attack OOM (Out Of Memory)

At the early stage of my career there were answers for OOM all over sites like stackoverflow and Android blogs on 
how to scale down the image or how to load bitmap efficiently into the memory. 

Still on profound usage of application crashlytics reported OOM issue persists. 

I realized that size of the image alone doesn't contribute to OOM, In some rare cases, 
leaked classes can even stick around for long enough to receive registered 
callbacks, causing some really strange bugs and all too often throw the notorious IllegalStateException. 

{% gist bd9f058084d56885d1bdae3bdd309649 %}
