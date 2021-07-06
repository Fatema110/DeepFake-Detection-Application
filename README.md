# DeepFake-Detection-Application Using Django #



In recent years, deepfake technology has made huge leaps in terms of accuracy, quality, and most of all: believability. At one time or another, we've all been fooled by a computer-generated viral image or even someone's Snapchat filter. The ability to determine whether or not an image is reality is quickly becoming a necessity in a world that's becoming more and more susceptible to "questionable" information. Recently, doctored images have made headlines and divided people in their opinions of whether real-world issues were legitimate. In this project we have built a video classification system that can determine if it is real or deepfake. The propose system detects the DeepFake using **Convolutional Neural Network (CNN)** and **Recurrent Neural Network (RNN).**


In a narrow definition, deepfakes (stemming from “deep learning” and “fake”) are created by techniques that can superimpose face images of a target person onto a video of a source person to make a video of the target person doing or saying things the source person does. This constitutes a category of deepfakes, namely face swap. 
In a broader definition, deepfakes are artificial intelligence (AI)-synthesized content that can also fall into two other categories, i.e., lip-sync and puppet-master. 
Lip-sync deepfakes refer to videos that are modified to make the mouth movements consistent with an audio recording. 
Puppet-master deepfakes include videos of a target person (puppet) who is animated following the facial expressions, eye and head movements of another person (master) sitting in front of a camera

## Requirements:

Note : **Nvidia GPU** is mandatory to run the application.

You can find the list of requirements in requirements.txt. Main requirements are listed below:

**Python >= v3.6
Django >= v3.0**

## Directory Structure ##

* ml_app -> Directory containing code in views.py file
* project_settings -> Contains Django settings and files to run in production
* static -> Contains all css, js and json files (for face-api)
* templates -> Template files for HTML

Note: Before running the project make sure you have created directories namely models, uploaded_images, uploaded_videos in the project root and that you have proper permissions to access them.

### Prerequisite ###
Copy your trained model to the models folder.
You can download our trained models from the [Google Drive ](https://drive.google.com/drive/folders/1UX8jXUXyEjhLLZ38tcgOwGsZ6XFSLDJ-?usp=sharing "Google Drive")or you can train your models using the steps mentioned in Model Creation directory.

* Step 1 : Clone the repo and Navigate to Django Application
  git clone https://github.com/Fatema110/DeepFake-Detection-Application.git

* Step 2: Create virtualenv (optional)
  python -m venv venv

* Step 3: Activate virtualenv (optional)
  venv\Scripts\activate

* Step 4: Install requirements
  pip install requirements.txt

* Step 5: Copy Models
  Copy your trained model to the models folder i.e Django Application/models/

You can download our trained models from Google Drive
Note : The model name must be in specified format only i.e model_84_acc_10_frames_final_data.pt. Make sure that no of frames must be mentioned after certain 3 underscores _ , in the above example the model is for 10 frames.

* Step 6: Run project
  python manage.py runserver
