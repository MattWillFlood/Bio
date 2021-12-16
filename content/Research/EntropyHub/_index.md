---
title: "EntropyHub"
date: 2021-07-20T14:16:20+02:00
draft: false
description: "EntropyHub: An Open-Source Toolkit for Entropic Time Series Analysis"
cover: "img/EH1.png"
weight: 1

---

# [**EntropyHub**](https://www.entropyhub.xyz)

> [_**PLoS One publication on EntropyHub**_](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0259448)    
> [_**Press release for EntropyHub**_](https://researchluxembourg.lu/2021/12/09/entropyhub-an-open-source-toolkit-for-researchers-and-companies/)

[{{< figure src="../../img/EH3.png" position="center" style="width:150px; ">}}](https://www.entropyhub.xyz)

During my PhD studies, I employed nonlinear signal analysis methods to analyse physiological time series data.
Entropy was just one of these methods, which is commonly used to estimate the randomness/complexity/irregularity of data.
However, access to reliable, accurate, and validated software with which to perform entropic data analysis was lacking.
This was not just an issue for me and other early stage researchers, but for the scientific community as a whole.
Without a reliable resource for conducting data analysis with entropy, it became difficult to cross-validate and replicate results from various studies.

I set out to change this and ended up creating [EntropyHub - an open-source toolkit for entropic time series and image data analysis.](https://www.entropyhub.xyz)


[{{< figure src="../../img/plos1.png" position="center" style="width:600px; " >}}](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0259448)

# **About**

Over the last few decades, there has been an increasing number of studies employing measures of entropy to estimate the **irregularity/randomness/complexity** of time series and image data in real-world applications. Matching the rise in popularity of entropy, the number of new methods of estimating entropy has similarly increased to leave what has been recently termed, "The Entropy Universe".
This universe of entropies continues to expand as more and more methods are derived with improved statistical properties over their precursors, such as robustness to short signal lengths, resilience to noise, insensitivity to amplitude fluctuations. Furthermore, new entropy variants are being identified which quantify the variability of time series data in specific applications, including assessments of cardiac disease from electrocardiograms, and examinations of machine failure from vibration signals.

{{< figure src="../../img/mandelbrot.png" position="center" style="width:400px; " >}}

As the popularity of entropy spreads beyond the field of mathematics to subjects ranging from neurophysiology to finance, there is an emerging demand for software packages with which to perform entropic time series analysis. **Open-source software plays a critical role in tackling the replication crisis in science by providing validated algorithmic tools that are available to all researchers**. Without access to these software tools, researchers lacking computer programming literacy may resort to borrowing algorithms from unverified sources which could be vulnerable to coding errors. Furthermore, software packages often serve as entry points for researchers unfamiliar with a subject to develop an understanding of the most commonly used methods and how they are applied. This point is particularly relevant in the context of entropy, a concept that is often misinterpreted, and where the name and number variant methods may be difficult to follow. For example, derivatives of the original sample entropy algorithm, already an improvement on approximate entropy. include modified sample entropy (fuzzy entropy), multiscale (sample) entropy, composite multiscale entropy, refined multiscale entropy, and refined-composite multiscale entropy.

{{< figure src="../../img/lorenzjl.png" position="center" style="width:400px; " >}}

Several packages offering entropy-related functions have been released in recent years, intended primarily for the analysis of physiological data. Although these packages offer some useful tools, they lack the capacity to perform extensive data analysis with multiple methods from the cross-entropy, bidimensional entropy, and multiscale entropy families of algorithms. Additionally, the utility of these packages is also limited for several reasons. Nearly all operate through graphical user interfaces (GUIs) and/or are designed for use with the MATLAB programming environment which requires a purchased license in order to use. This paywall prevents many users from accessing the software and consequently impedes the replication of results achieved by using these packages. Few have accompanying documentation to describe how to use the software, and none are hosted on the native package repository for MATLAB (MathWorks File Exchange) or Python (PyPi), which facilitate direct and simplified installation and updating.


> Against this background, I developed EntropyHub, an open-source toolkit for entropic time series analysis in the [**MATLAB**](https://www.mathworks.com/matlabcentral/fileexchange/94185-entropyhub), [**Python**](https://pypi.org/project/EntropyHub/) and [**Julia**](https://juliahub.com/ui/Packages/EntropyHub/npy5E/) programming environments. Incorporating entropy estimators from information theory, probability theory and dynamical systems theory, EntropyHub features a wide range of functions to calculate the entropy of, and the cross-entropy between, univariate time series data. In contrast to other entropy-focused toolboxes, EntropyHub runs from the command line without the use of a GUI and provides many new benefits, including:

* Functions to perform _**refined, composite, refined-composite and hierarchical multiscale entropy**_ analysis using more than twenty-five different entropy and cross-entropy estimators (approximate entropy, cross-sample entropy, etc).    
* Functions to calculate bidimensional entropies from _**two-dimensional (image) data**_.      
* An extensive range of function arguments to specify additional parameter values in the entropy calculation, including options for _**time-delayed state-space reconstruction**_ and entropy value normalisation where possible.      
* Availability in multiple programming languages – [**MATLAB**](https://www.mathworks.com/matlabcentral/fileexchange/94185-entropyhub), [**Python**](https://pypi.org/project/EntropyHub/) and [**Julia**](https://juliahub.com/ui/Packages/EntropyHub/npy5E/) – to enable open-source access and provide cross-platform translation of methods through consistent function syntax. **This is the first entropy-specific toolkit for the Julia language, and the first package of its kind to be available in all three languages.**      
* Compatible with both _**Windows, Mac and Linux**_ operating systems.     
* _**Comprehensive documentation**_ describing installation, function syntax, examples of use, and references to source literature. Documentation is available online at [www.EntropyHub.xyz](www.EntropyHub.xyz) (or at [MattWillFlood.github.io/EntropyHub](www.EntropyHub.xyz)), where it can also be downloaded as a booklet (**EntropyHub Guide.pdf**). Documentation specific to the MATLAB edition can also be found in the ‘supplemental software’ section of the MATLAB help browser after installation. Documentation specific to the Julia edition can also be found at [MattWillFlood.github.io/EntropyHub.jl/stable](MattWillFlood.github.io/EntropyHub.jl/stable).     
* Hosting on the native package repositories for MATLAB (MathWorks File Exchange), Python (PyPi) and Julia (Julia General Registry), to facilitate _**straightforward downloading, installation and updating**_. The latest development releases can also be downloaded from the EntropyHub GitHub repository - www.github.com/MattWillFlood/EntropyHub.   

As new measures enter the ever-growing entropy universe, EntropyHub aims to incorporate these measures accordingly. 

EntropyHub is licensed under the Apache license (version 2.0) and is available for use by all on condition that the following reference be cited on any scientific outputs realised using the EntropyHub toolkit.  

    Matthew W. Flood and Bernd Grimmm, (2021)
    EntropyHub: An open-source toolkit for entropic time series analysis
    PLoS One 16(11):e0259448
    DOI: 10.1371/journal.pone.0259448

# Download EntropyHub from:

| [{{< figure src="../../img/GH2.png" style="width:100px;" position="center">}}](https://github.com/MattWillFlood/EntropyHub) | [{{< figure src="../../img/Matlab_Logo.png" style="width:100px; " position="center">}}](https://www.mathworks.com/matlabcentral/fileexchange/94185-entropyhub) | [{{< figure src="../../img/pythonlogo.png" style="width:100px; " position="center">}}](https://pypi.org/project/EntropyHub/)  |  [{{< figure src="../../img/julialogo.png" style="width:100px; " position="center" >}}](https://juliahub.com/ui/Packages/EntropyHub/npy5E/) | [{{< figure src="../../img/EH1.png" style="width:100px;" position="center">}}](https://www.EntropyHub.xyz)  |
|----|----|----|----|----|

# Links:

* [EntropyHub Website](https://www.entropyhub.xyz)
* [EntropyHub Journal Paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0259448)
* [GitHub repository](https://github.com/MattWillFlood/EntropyHub)
* [MatLab download centre](https://www.mathworks.com/matlabcentral/fileexchange/94185-entropyhub)
* [Python package repository](https://pypi.org/project/EntropyHub/)
* [Julia package registry](https://juliahub.com/ui/Packages/EntropyHub/npy5E/)

> * [Press coverage on EntropyHub](https://researchluxembourg.lu/2021/12/09/entropyhub-an-open-source-toolkit-for-researchers-and-companies/)


