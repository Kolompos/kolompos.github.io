---
layout: page
title: RF MUX-DEMUX
description: Major component in a big RF system.
img: assets/img/MUX-DEMUX.jpg
importance: 1
category: work
---

[← Back]({{ site.url }}/projects/)

Although most parts of this project were and are still classified, I can elaborate without being too specific.

The company <a href="https://sagaxcommunications.com/">Sagax Communications</a> has a main portfolio around <a href="https://en.wikipedia.org/wiki/Software-defined_radio">SDR</a> equipment. They develop and maintain specialized hardwares for signal processing and also softwares for user interface. They are also providing <a href="https://en.wikipedia.org/wiki/Radio-frequency_engineering">RF</a> hardware for signal conditioning. Switching, splitting, amplifying, filtering and more.


<div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
    {% include figure.html path="assets/img/MUX-DEMUX.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    Exact configuration of the MUX-DEMUX can't be disclosed, this is just an illustration.
</div>


The big RF system consisted of signal sources and SDRs. The signals had to be channeled to the SDRs in a flexible way. This task required a complex MUX-DEMUX matrix. The inside of the matrix consisted of hundreds of <a href="https://en.wikipedia.org/wiki/RF_connector">connectors</a>. Although the main concept and architecture of the matrix was already designed when I joined the project, I helped with the fine tuning of the design to the costumers requirements.

One of my tasks was to document the positions and pairs of all these ports. I did this in <a href="../skills/autocad.html">AutoCAD</a>. The final drawing was a custom length A1 print. As it would have been impossible to manually name every port, I used excel to generate the names of all the ports, exported to CSV and imported that into AutoCAD.

The matrix had to be controlled and I got the opportunity to make the controller circuits. The RF design was made by a colleague but he was not familiar with digital control circuits. Following his design's requirements, I prototyped and tested the controllers and then integrated it into the system.


<div class="text-center">
    <a href="{{site.url}}/projects/">
        <button type="button" class="btn">Projects</button>
    </a>
</div>