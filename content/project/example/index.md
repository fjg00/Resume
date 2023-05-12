---
title: Shared Control in Autonomous Vehicles
summary: Enhancing user's trust in autonomous driving by developing efficient human-machine interfaces that predict the user's intentions and prompts for handback.
tags:
  - Deep Learning
date: '2023-05-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: CARLA Simulator Setup
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Driver safety is a major concern for the automotive industry today, and researchers and industries are exploring the introduction of self-driving vehicles as a solution. These vehicles aim to assist drivers during their journeys, making them more enjoyable, safe, and efficient. Despite the introduction of new features to self-driving vehicles, many people still do not trust them enough and prefer to be in control of the driving experience. This lack of trust can be attributed to various factors, such as the lack of information about automated vehicles, poor communication with the automation, or people being unaware of the full capabilities of the system.

To address this issue, we propose a human-machine interface (HMI) that facilitates the process of hand-back and takeover between the driver and the vehicle. Our HMI leverages inputs from the Controller Area Network (CAN) bus of the car to predict the driver's intentions accurately and display them in a safe and user-friendly manner. We evaluated several predictions, such as identifying whether the driver is stuck in traffic or attempting to parallel-park.
As our project involves the safety of drivers and passengers, we must comply with several standards and constraints. Our system must make accurate predictions in real-time while running on a local device, adhering to various standards set by associations such as SAE, NHTSA, and ITU.

We used the CARLA (Car Learning to Act) Simulator to simulate real-world traffic scenarios and parallel parking situations, collecting data such as throttle, brake, speed, steering wheel angle, and reverse signals for analysis. This analysis enabled us to develop and test various machine learning models, ultimately choosing the models with the highest accuracy. We then designed an HMI that adheres to the relevant standards and effectively communicates the predictions to the driver. We conducted experiments on the CARLA Simulator and administered a questionnaire to assess the performance of the HMI and the predictions. 
