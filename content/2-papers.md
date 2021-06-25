Title: GIRAFFE: Representing Scenes as Compositional Generative Neural Feature Fields
Date: 2021-06-25 16:12
Category: Paper
Tags: Paper, Summary, Research

Authors:- Niemyer/Geiger et al. 

Summary of the following [Paper](https://arxiv.org/pdf/2011.12100.pdf):-

* Hypothesis:- Incorporating a compositional 3D scene representation into generative models leads to controllable image generation.

* Model allows for disentangled individual objects and allows for translating and rotating them in the scene, as well as changing camera pose. 

* Model claimed to generalize beyond training data, i.e. Can sythesize images not in training data -- more objects etc etc. 

* Combining an explicit 3D representation with neural rendering pipeline results in faster inference and more realistic images. 

* Most 3D neural renderers need camera pose as supervision, but this technique learns it from unstructured image collections. 

<b>Pros</b>

* Can render scenes in a compositional manner.

* The scenes are realistic. 

* Does not use implicit supervision, and instead learns from unstructured sets of images. 

* Use 3D models of scenes rather than 2D images to learn. 

<b>Cons</b>

* Biases which are implicit in the datasets, do not get untangled during learning factors of variation. 

* For every parameter of variation, explicit control mechanisms need to provided at training time to learn them, i.e. Factors of variation are not learned explicitly. 

* The factors of variation probably influence the number of parameters -- despite the authors working in lower dimensional pixel space. 
 
