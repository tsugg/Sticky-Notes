# Sticky-Notes

Here is my attempt at the AFS Challenge #24 

I tried to make it as easy as possible for anyone to reproduce my expirement, so I've decided to use Google Colab. I was having issues with cudnn versions when I tried to run the code on multiple devices on Jupyter Notebook.

I took about 20 images of different colored sticky notes on a white wall. Each image had anywhere between 5 and 15 sticky notes.

I decided to use ImageAI's custom object detection API, since this was a pretty quick challenge. I didn't want to get stuck in hours of training custom CNNs.
The documentation can be found here : https://imageai.readthedocs.io/en/latest/customdetection/

This was my first attempt at using OCR, so I wasn't quite sure which API to use. I went with keras-ocr since I am comfortable using that framework. If you have any advice on other algorithms to use please let me know. 
The documentation can be found here : https://github.com/faustomorales/keras-ocr

# INSTRUCTIONS

## Step 1: Download the model 
Download from here: https://drive.google.com/open?id=1waRi2YBuNY6pX7kCYy_kWsI0AylFpYco

## Step 2: Go to the Google Colab Notebook
Download from here : https://drive.google.com/open?id=1Qc1E8z0MPUzzVZIeFxlGACtgFJP2tQH_
and upload it to colab.research.google.com
(You can also open it directly from the master branch)

## Step 3: Follow instructions on the Google Colab notebook
