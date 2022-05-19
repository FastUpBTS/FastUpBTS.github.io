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

[Representitive BTSes](#representitive-btses)

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

## Representitive BTSes
