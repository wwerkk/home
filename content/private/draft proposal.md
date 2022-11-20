---
title: "Draft Proposal"
---
# Sequence modelling for concatenative audio synthesis
 [![ "PLAYSTATION STARTUP," Continued by a Neural Network (OpenAI's Jukebox)](https://img.youtube.com/vi/VaQHa3pKajU/0.jpg)](https://www.youtube.com/watch?v=VaQHa3pKajU)

## Topic
Concatenative audio synthesis has a long history of introducting ML methods to creative sound practices. Corpus-Based Concatenative Synthesis toolboxes such as IRCAM's CataRT as well as FluCoMa package developed at University of Huddersfield both provide advanced tools for audio segmentation, analysis and resynthesis.
[samplebrain](https://gitlab.com/then-try-this/samplebrain) is a tool in a similar vein, created in collaboration between Aphex Twin and Dave Griffiths.

More recently, neural networks based on autoencoder architecture have proved themselves capable of audio generation with almost-approachable performance requirements with their implementations such as [Musika!](https://marcoppasini.github.io/musika) coming out of University Linz and [RAVE](https://github.com/caillonantoine/RAVE) from ACIDS team at IRCAM (again), both possible to train on consumer gaming GPUs.
Both of these deal with compactily encoding (spectral or other) representations of audio frames (which are indeed segmented, similar as in Corpus Analysis), and then modelling that representation with the purpose of reversing the process, enabling generation of audio of arbitrary length.

None the less, the latter still do require substantial amounts of training data and prove way more computationally expensive than the *classic*, sample-based concatenative approaches, considering they synthesize audio samples from scratch.
The possibility of hybridization of these techniques is the basis for my inquiry.

## Research question
Can advanced methods used for modelling and generation of temporal series (such as audio signal) be successfully appropriated into concatenative synthesis tools and potentially reduce the amount of data/computational power required for audio generation?


![diagram.png](diagram.png)

## Project timeline

| November | December | January | February | March | April | May
|-|-|-|-|-|-|-|
| naive prototype (SuperCollider/MaxMSP) | sequence modelling | SCA implementation attempt | online/offline implementations (SuperCollider/Python/Torch Script?) | GUI attempt/brush up/write up | brush up/write up | finalize