---
title: Water Safety with Computer Vision
summary: Computer vision system able to locate and identify specific entities on live drone footage, such as persons, dangerous currents and more.
tags:
- Deep Learning
- Computer Vision
date: "2021-09-09T08:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Computer vision (CV) is the science allowing computers and software systems to gain high-level understanding from digital images or videos. While a wide variety of tasks span from this discipline, they usually all share the general end goal of extracting specific information that will be useful in a broader production process. 


For this project, we focused on the object recognition task, which refers to the capability to locate and identify specific objects. With SN Hawaii and Waterman5, we developed a water safety computer vision system, able to locate key entities on live drone footage, such as persons, dangerous currents, surfers and more.


{{< video src="ai_ocean_safety.mp4" controls="yes" >}}


Modern computer vision systems rely almost exclusively on deep neural networks (deep learning), due to their high performance, which stems from their inherent capability to learn and generalize well on big datasets. Whereas traditional deep learning systems require millions of identified examples, and heavy computing resources to reach desirable production performance, we avoided these major drawbacks in the present case by using transfer learning. Transfer learning is a research branch of artificial intelligence, which consists in exploiting learned knowledge from an existing system, to apply (transfer) it in a new (connex) setting. 


More concretely, instead of training a new model from scratch, with many labeled examples, we started from an existing state-of-the-art research CV model that was already trained for months on a gigantic dataset and accelerated with multiple GPUs. Our goal was to keep all the neural network’s learned treatment and analysis capabilities, but to change it’s end goal to predict our objects instead of the ones it was originally designed to. By doing so, by providing only a handful of annotated images specific to our application, we were able to achieve the performance shown in the video above. Even better ! The training only took a few hours, on an every-day laptop with no GPU. Imagine the possibilities.

{{< figure src="labeling.png" caption="Labeling process to train the computer vision system. Only a handful of these examples are necessary to obtain the performance shown above." numbered="false" >}}