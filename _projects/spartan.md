---
layout: page
title: SPARTAN and SEDOBS
description: Galaxy fitting tools
img: assets/img/project/spartan/transparent.png
importance: 3
category: work
related_publications: true
---


This is one of the first big software I created for my research. It was a tool that was doing photometry and spectroscopy fitting for galaxy data. In short, you observe a galaxy with a telescope, and you try to estimate the physical parameters of this galaxy (such as age, metal content, star formation rate, dust content, etc...) by comparing it to a load of theoretical models. It took me quite some time to develop it.

You can find a bit more details in the poster below, that was presented at the EAS conference in Prague. 

<center>
<figure class="center">
<img src="../../assets/img/project/spartan/SPARTAN-prague-black.png" alt="And example of SEDOBS fake galaxy" style="max-width: 100%; height: auto;">
<figcaption color=white>EWASS poster</figcaption>
</figure>
</center>



The documentation is public and hosted on [GitHub](https://astrom-tom.github.io/SPARTAN/build/html/index.html). SPARTAN has been published in Astronomy and Computing {% cite Thomas_2021ac %}}

To test SPARTAN and its accuracy I made a software that creates galaxy simulations. The idea is to take the theoretical modesl and creates fake observation with them. Thois code is called SEDOBS. The user can create various mock observation spanning a large range of parameters. It also simulated pre-defined instruments that exists in real life so it is easy to look at various combination of observations.  

<center>
<figure class="center">
<img src="../../assets/img/project/spartan/sedobs.png" alt="And example of SEDOBS fake galaxy" style="max-width: 100%; height: auto;">
<figcaption color=white>An example of fake galaxy observation made by SEDOBS.</figcaption>
</figure>
</center>

SEDOBS as well is on GitHub with its full [documentation](https://astrom-tom.github.io/SEDobs/build/html/index.html) and published in Astronomy and Computing {% cite Thomas_2020ac %}.
