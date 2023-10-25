# Pravaas-Derailment-Prevention-by-Track-Object-Detection(IBMZ Datathon Submission)
## Inspiration
We are all aware of the rising number of railroad accidents, which can cause both property loss and fatalities. Derailments, which are now the primary cause of these accidents, are just one of the many reasons why this happens. Research indicates that derailments are responsible for *70 out of every 100 rail accidents.* 

Train derailments caused by foreign item invasions and track-related issues are a recurring problem in India. The railway network is severely disrupted by these derailments, endangering passengers' safety as well as the economy. 

## What it does
There is a critical need for an advanced monitoring system that provides real-time tracking of track conditions and detects concerning objects on the tracks. This system will efficiently detect objects that pose harm on the tracks, promptly informing the driver and authorities in advance.

For that, using *YOLOv5* as a Machine learning model which was trained on the custom dataset of various train tracks, the model is able to perform -

- *Object Detection* : The models is trained to analyze images or video footage from cameras installed along railway tracks. The models can identify and locate objects or obstacles on the tracks, such as fallen trees, rocks, debris, and even actual humans.

- *Real-time Monitoring*: The project involves monitoring of the railway tracks, and when an object or obstacle is detected, it will triggers an immediate response, such as notifying railway stations, signaling the train to slow down or stop, or initiating track maintenance. The model works for images as well as videos.

## How we built it
We went with YOLOv5 which is a vision AI model as the base model on which the training was done. We also created our own *custom dataset* of train obstacles to train the model. Creating the custom dataset involved selecting images from different sources and manually labelling them. The dataset had two parts the training part and the test part, which was further divided into the actual images on which the model was trained and the labeled. 

The model was trained in the *LinuxOne* and *Jupyter Notebook* environment. To train this model, we used a comprehensive suite of libraries, including but not limited to *OpenCV, tqdm, torch, and util*. These libraries played an indispensable role in ensuring the successful training of our custom model

Upon integrating the dataset into our workflow, we started to train on our customized *YOLOv5* model, utilizing the *COCO128* dataset as a benchmark. The training was executed over *two batches* spanning *300 epochs. Notably, our model achieved a remarkable accuracy rate of **89.5%*. Our intention was to further maximize the model's potential; however, due to time constraints, we were compelled to conclude our training at this stage.

## Challenges we ran into
The biggest difficulty was selecting the best model to use for data training. There were many choices, and each one was superior in its own way, but we settled on YOLOv5 as the model. The YOLOv5 was selected because it offered excellent community support and high throughput. Since this was our team's first machine learning project, we encountered numerous problems and coding errors. 

Because we couldn't locate a suitable dataset on Kaggle or other platforms, creating the custom dataset was rather difficult. Since the dataset is the most crucial component of any model, we decided to make our own unique dataset. We personally selected and labeled over *60 photos by hand*. One of the factors contributing to the high accuracy rate is the perfect dataset being chosen for the application.

## Accomplishments that we're proud of
We are proud that the accuracy of our very first machine learning project is a staggering 89.5%. The model produced a high accuracy rate because it swiftly adjusted to the specific dataset on which it was trained. Less mistakes and more accurate outcomes are the results of a high accuracy rate.

We're especially pleased that the model is able to spot mistakes in videos in addition to images. Since it will be used in a train station, it should be able to recognize from the video. 

## What we learned
This was the first AI/ML hackathon that our team has ever participated in, and we have learned a lot. We have thoroughly investigated this field, from topic research to model finalization and training. This project gave us the opportunity to learn about four areas, which will undoubtedly be helpful to us in the future: choosing the right model, training it, choosing the right dataset, and improving its performance.

## What's next for Pravaas - Derailment Prevention by Track-Object Detection
We have listed out a few changes or features we will add in future:
1. *Fine-Tuning and Optimization*: We'll be Continuously fine-tuning the YOLOv5 model to improve its accuracy and efficiency.
2. *Scalability*: We'll be making so that the system can be scaled to monitor larger sections of railway networks. 
3. *Integration with Rail Infrastructure*: Exploring ways to integrate the object recognition system with existing rail infrastructure, such as signal systems, traffic control centers, and automatic braking mechanisms, to ensure coordinated responses to detected obstacles.
4. *Data Augmentation*: Increasing the diversity and size of the dataset used for training. Incorporate data from various sources and environments to make the model more robust.
