# ARS_Finetune_demo

## Prerequisite
- Python
- Flask (`pip install Flask`)
- Chrome Web Browser

## Install instruction
- Clone this git `git clone https://github.com/mahmed10/ARS_Finetune_demo.git`
- Go to the directory `cd ARS_Finetune_demo`
- Run the py file `python app.py`
- Open the web browser
- Go to the following address `localhost:5000`

## Overview
Click the following video to see the full demo

[![Demo Video](http://img.youtube.com/vi/22EMXAfQhD8/0.jpg)](http://www.youtube.com/watch?v=22EMXAfQhD8)

## Functionality of the demo
There are seven button, which performs different task of the demo.
- **Start Segmentation:** Perform segementation on Real-time and display the result at user endpoint
- **Stop Segmentation:** Stop the semantic segmentation
- **Transfer Data:** Transfer data from the robot to user end
- **Start Annotation:** User can annotate the data at user endpoint
- **Stop Annotation:** Annotation process will be stopped
- **Start FineTune:** Server will start fine-tunning the model with annotated data
- **Transfer Model:** Updated model will be transfered to the robot from server

## Storyline
In a world where robots are indispensable for various tasks, especially in traversing unknown territories, there exists a challenge: the transition from urban to rural environments often leads to performance degradation in semantic segmentation models. To tackle this issue, we embarked on a journey to create a solution: the ARS_Finetune_demo.

At its core, ARS_Finetune_demo is an innovative web-based application designed to fine-tune semantic segmentation models on-the-fly with minimal labeled data from rural environments. The journey begins with the deployment of a robot into real-time environments, where it encounters diverse landscapes and scenarios.

The demo unfolds through an intuitive interface, accessible via a web browser. Seven buttons serve as gateways to different functionalities of the demo, each playing a pivotal role in the overarching narrative:

1. **(Click Start Segmentation button):** The robot initiates semantic segmentation in real-time whenever the user clicks the Start Segmentation button, capturing the essence of its surroundings and displaying the results at the user's endpoint.
2. **(Click Stop Segmentation button):** When needed, the segmentation process can be halted, allowing for control and precision in data acquisition.
3. Here, you can observe that the robot is not performing well.
4. It's important to note that when the robot performs inference, it also keeps track of the performance based on entropy. Based on entropy calculation, it will keep track of the hard images and the hard regions of those images where the model is not performing well.
5. If a user wants, they can fine-tune the model on the fly with a small fraction (approximately 5%) of those hard images' hardest regions.
6. **(Click Transfer Data button):** When a user presses the Transfer Data button, the robot seamlessly transmits those hard regions of those hard samples to the user's endpoint, laying the groundwork for further analysis and refinement.
7. **(Click Start Annotation button):** Upon receiving this data at the user's endpoint, the user can annotate those hard regions so that the model can be fine-tuned with this data.
8. **(Click Stop Annotation button):** With annotation complete, this button signifies the conclusion of the user's input phase, preparing the stage for model fine-tuning.
9. **(Click Start FineTune button):** After finishing annotation, when the user presses this button, the server comes into action, leveraging the annotated data to fine-tune the semantic segmentation model, adapting it to the nuances of rural environments.
10. **(Click Transfer Model button):** As the climax of the narrative unfolds, the updated model is transmitted back to the robot from the server, equipped with newfound knowledge and capabilities to navigate and understand its surroundings more effectively.
--- 

Through a captivating demo video, viewers are invited to witness this transformative journey, where innovation meets necessity, and technology paves the way for seamless adaptation and enhanced performance in the ever-evolving landscape of robotics and AI.
