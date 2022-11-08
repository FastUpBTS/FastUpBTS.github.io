<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>
<br />
<center style="font-size:45px;color:green;"> Fast Uplink Bandwidth Testing for Internet Users </center>

![license](https://img.shields.io/badge/platform-web-green "Web")
![license](https://img.shields.io/badge/Version-Beta-yellow "Version")
![license](https://img.shields.io/badge/Licence-Apache%202.0-blue.svg "Apache")

## Table of Contents
[Introduction](#introduction)

[FastUpBTS We Implement](#fastupbts-we-implement)

[Representitive BTSes We Reimplement for Fair Comparison](#representitive-btses-we-reimplement-for-fair-comparison)

## Introduction
Access bandwidth measurement is crucial to emerging Internet applications for network-aware content delivery.
However, today's bandwidth testing services (BTSes) are slow and costly---the tests take a long time to run, consume a great deal of data usage, and usually require large-scale test server deployments.
The inefficiency and high cost of BTSes root in their methodologies that use excessive temporal/spatial redundancies for combating noises in Internet measurement.
In particular, compared to downlink BTSes, uplink BTSes are subject to more severe performance problems and technical challenges.
This paper presents FastUpBTS to make uplink BTS fast and cheap while maintaining high accuracy.
The key idea is to strategically accommodate and exploit the noise rather than repetitively and exhaustively suppress the impact of noise.
This is achieved by a novel statistical sampling framework termed *fuzzy rejection sampling*.
We build FastUpBTS as an end-to-end BTS that implements fuzzy rejection sampling based on memorization-reinforced throughput denoising, data-driven server selection, and informed multi-homing support.
Our evaluation shows that with only 30 test servers, FastUpBTS achieves the same level of accuracy compared to the state-of-the-art BTS (SpeedTest.net) that deploys ~16,000 servers.
Most importantly, FastUpBTS makes bandwidth tests 5.4$\times$ faster and 6.8$\times$ more data-efficient.

## FastUpBTS We Implement


<style>
table th:nth-of-type(1) {
    width: 100px;
    max-width:100px;
    min-width:100px;
}
</style>

|BTS|Implementation|
|:----:|------|
|FastUpBTS|[https://github.com/FastUpBTS/FastUpBTS/tree/main/FastUpBTS](https://github.com/FastUpBTS/FastUpBTS/tree/main/FastUpBTS)|

## Representitive BTSes We Reimplement for Fair Comparison
<style>
table th:first-of-type {
    width: 20%;
}
table th:nth-of-type(2) {
    width: 40%;
}
table th:nth-of-type(3) {
    width: 40%;
}
</style>
|BTS|Website|Implementation|
|:----:|------|------|
|ThinkBroadBand|[https://www.thinkbroadband.com](https://www.thinkbroadband.com)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/TBB](https://github.com/FastUpBTS/FastUpBTS/tree/main/TBB)|
|SpeedOf|[https://speedof.me](https://speedof.me/)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/SpeedOf.me](https://github.com/FastUpBTS/FastUpBTS/tree/main/SpeedOf.me)|
|BWP|[https://www.bandwidthplace.com](https://www.bandwidthplace.com/)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/BWP](https://github.com/FastUpBTS/FastUpBTS/tree/main/BWP)|
|Xfinity|[http://speedtest.xfinity.com/](http://speedtest.xfinity.com)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/XFinity](https://github.com/FastUpBTS/FastUpBTS/tree/main/XFinity)|
|FAST|[https://fast.com](https://fast.com)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/FAST.com](https://github.com/FastUpBTS/FastUpBTS/tree/main/FAST.com)|
|SpeedTest|[https://speedtest.net](https://speedtest.net)|[https://github.com/FastUpBTS<br>/FastUpBTS/tree/main/SpeedTest.net](https://github.com/FastUpBTS/FastUpBTS/tree/main/SpeedTest.net)|
|LibreSpeed|[https://librespeed.org/](https://librespeed.org/)|[https://github.com/librespeed/speedtest<br>(directly use the open-source version)](https://github.com/librespeed/speedtest)|