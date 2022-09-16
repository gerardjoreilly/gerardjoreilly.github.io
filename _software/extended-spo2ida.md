---
title: "Extended SPO2IDA for Infilled RC Frames"
excerpt: "Compute the IDA curves for non-ductile RC frames with masonry infills using just the results of pushover analysis"
collection: software
---

## Overview
SPO2IDA has emerged as a convenient tool for the assessment of structures. It relates a structure’s static pushover analysis (SPO) results to incremental dynamic analysis (IDA) curves using a library of empirical fitting coefficients for the different branches of the idealised SPO backbone, as shown below. It permits the quantification of structural performance up to structural collapse as a function of seismic intensity in a simple and efficient manner.

<img src="/images/spo2ida.jpg" style="width:48px;height:48px;">

## Behaviour of Infilled RC Frames
It has been developed for ductile structures that can be represented via a SPO backbone with a ductile post-yield hardening followed by a post-peak degradation, as shown above. This behaviour is quite representative of ductile RC and steel moment-resisting frames and has resulted in the tool being widely adopted.

However, considering the peculiar behaviour of infilled RC frames (below) where a high strength and stiffness contribution from the infill panels is initially present. Upon the local collapse of a storey's infill panels, and the formation of a weak storey mechanism (below), the strength and stiffness properties of the frame change significantly, which has a notable impact in the seismic response up to collapse. It is this feature that Extended SPO2IDA incorporates.

<img src="/images/infilled-rc.jpg" style="width:48px;height:48px;">

## Extension of SPO2IDA to Infilled RC Frames
A new library of empirical coefficients have been fitted and proposed by considering a large database of representative backbones to result in an Extended SPO2IDA proposal for infilled RC frames. Comparison with actual IDA shown below illustrate the effectiveness of the tool.

<img src="/images/extended-spo2ida-example.jpg" style="width:48px;height:48px;">

This has also been verified through a case study application to an existing school building in Italy, shown below. A static pushover analysis of the building was carried out (below left) and the Extended SPO2IDA was utilised. The result (below right) was a set of fragility curves for the building limit states obtained from Extended SPO2IDA. When compared with fragility functions obtained using extensive non-linear dynamic analyses with hazard-consistent ground motion records, the accuracy of the simplified tool is apparent.

<img src="/images/extended-spo2ida-example2.jpg" style="width:48px;height:48px;">

For the latest version of the tool, please visit the Github page [here](https://github.com/gerardjoreilly/InfilledRC-SPO2IDA).

## Relevant references:
1. Nafeh AMB, **O’Reilly GJ**, Monteiro R. Simplified seismic assessment of infilled RC frame structures. Bulletin of Earthquake Engineering 2020; 18(4): 1579–1611. DOI: 10.1007/s10518-019-00758-2. [[PDF](http://gerardjoreilly.github.io/files/Journal/J13-2020_Nafeh, O’Reilly, Monteiro_Simplified seismic assessment of infilled RC frame structures.pdf)][[Link](https://link.springer.com/article/10.1007/s10518-019-00758-2)]
