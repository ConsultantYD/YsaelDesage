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

Computer vision (CV) is the science allowing computers and software systems to gain high-level understanding from digital images or videos. While a wide variety of tasks span from this discipline, they usually all share the general end goal of extracting specific information that will be useful in a broader production process. Typical successful examples of applied computer vision include self-driving cars, facial recognition or even medical imaging diagnosis.


For this project, focus is given to the object recognition task, which refers to the capability to locate and identify specific objects. With SN Hawaii and Waterman5, we developed a water safety computer vision system, able to locate key entities on live drone footage, such as people, dangerous currents, surfers and more.


{{< video src="ai_ocean_safety.mp4" controls="yes" >}}


Modern computer vision systems rely almost exclusively on deep neural networks (deep learning) due to their high performance which stems from their inherent capability to learn and generalize well from big datasets. Whereas traditional deep learning systems require millions of identified examples and heavy computing resources to reach desirable production performance, these major drawbacks were avoided in the present case by using transfer learning. Transfer learning is a research branch of artificial intelligence which consists in exploiting learned knowledge from an existing system to apply (transfer) it in a new (connex) setting. 


More specifically, instead of training a brand new model from scratch (which would require many labeled examples), the starting point of the project was an existing state-of-the-art model that was already trained on a gigantic dataset. The final goal was to keep all the cutting-edge neural network’s self-taught treatment and analysis capabilities, but to simply change its end goal to locate our objects instead of the ones it was originally designed to. By doing so, only a handful of annotated images that are specific to our application, and a little fine-tuning were necessary to achieve the performance in the video shown above. Even better, the training only took a few hours, and was executed on a normal laptop with no GPU or specialized hardware acceleration.

{{< figure src="labeling.png" caption="Labeling process to train the computer vision system. Only a handful of these examples are necessary to obtain the performance in the video shown above." numbered="false" >}}

Do not hesitate to reach out to discuss the potential of computer vision or other methods for your own application.