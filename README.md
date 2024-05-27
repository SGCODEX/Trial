# **Readme File:**
1) I have uploaded all the data, python files, runs, dockerfile and rest to a drive for training on Google Colab and easy accessibility.
drive link: https://drive.google.com/drive/folders/1MmzIOpMC4wmuZ6tP5SGf-Z2WWGHdzp8e?usp=sharing
2) Annotated dataset is divided into 3 parts for training the model: train, test and val using python script **Python Codes\Split.py**: https://drive.google.com/file/d/1txxb4FYaCfMBHEE3xEn1DIlMLoOXdwf5/view?usp=drive_link
3) Now with help of **pandas** I cleaned the data and created a new csv called train_cleaned.csv, keeping only the classes required using **Python Codes\Dataclean.ipynb**: https://drive.google.com/file/d/1Nfboxg7mxEL2sN8RNo3KekBIb3YLZp45/view?usp=sharing
4) Finally the model was custom trained on Yolov8n model using the following **Google Colab Notebook**: https://colab.research.google.com/drive/1xCVDLzoMuPOA7IRGTNxor4J1SNZDpIUj?usp=sharing
<br>*Problems Faced:* 1)Due to low availability of time and hardware resources (such as limited availability of GPU on Google Colab), I had to train model for lower number of epoch cycles (5) and increase the batch size. Thus leading to lower accuracy than expected but the model can be trained for more number of epochs again using best.pt
5) **Task 1**:Now using the custom trained model we saved the results in submission.csv and also saved the predicted the images 1 - 1800: https://drive.google.com/drive/folders/1MFlMterqNgfuAhajA4kZYOiX0RPDwDpX?usp=drive_link
6) **Task 2**:Again using the custom model, we have predicted nd tracked the output videos. Attached in the mail or can be viewed here: https://drive.google.com/drive/folders/10IfQazlL2NuqNvTI4hMWp4UcTVB87lfI?usp=drive_link
7) Finally created a docker file and an app.ipynb to create a docker image.
<br> -> Docker image is pushed to the hub: [https://hub.docker.com/repository/docker/shivamguptadtc/mask-wobotai](https://hub.docker.com/r/shivamguptadtc/mask-wobotai)
<br> -> Pull using this command: docker pull shivamguptadtc/mask-wobotai:0.1
<br> -> Run using this command: docker run -it -p 8888:8888 shivamguptadtc/mask-wobotai:0.1

Note: I have also mentioned the in-deapth approach I have followed in Google Colab as well.
