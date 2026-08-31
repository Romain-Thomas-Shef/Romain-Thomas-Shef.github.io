---
layout: page
title: Photon
description: An interface to make paper ready plots
img: assets/img/project/photon/photon1.png
importance: 5
category: work
related_publications: true
---

I got so tired of rewriting the similar codes over and over again to make plots that I have created a tool that makes them for me. 
Photon is a GUI created to make simple 1D plot in python. It uses mainly matplotlib and PyQt5 and it has been build in the spirit of being fully customizable. You can change fontstyle, fontsize, fontcolors, linewidth of the axes, thickness, etc…and see the changes directly in the plot. Once a customization is created, you can save it into a configuration file and reload it later when you open photon again. This allows you to keep the same customization for different plot. The main tool is a graphical user interface and it is started using a command line interface.

<center>
<div class='row justify-content-center text-center'>
    <div class='col-sm-6'>
        <figure class="center">
            <img src="../../assets/img/project/photon/photon1.png" alt="Example" style="width: 305px">
            <figcaption color=white>Example of plot</figcaption>
        </figure>
    </div>
    
    <div class='col-sm-6'>
        <figure class="center">
            <img src="../../assets/img/project/photon/photon2.png" alt="Example" style="width: 305px">
            <figcaption color=white>Example of plot</figcaption>
        </figure>
    </div>

</div>
</center>

The interface looks like this:

<center>
    <figure class="center">
        <img src="../../assets/img/project/photon/photon3.png" alt="Interface of Photon" style="width: 665px">
        <figcaption color=white>Interface of photon.</figcaption>
    </figure>
</center>

Photon is available in the Astrophysics Source Code Library {% cite 2019ascl.soft01007T %} and the documentation is on [GitHub](https://romain-thomas-shef.github.io/Photon/build/html/index.html).
