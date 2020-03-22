# Sticky-Notes

Here is my attempt at the AFS Challenge #24 

I tried to make it as easy as possible for anyone to reproduce my expirement, so I've decided to use Google Colab. I was having issues with cudnn versions when I tried to run the code on multiple devices on Jupyter Notebook. If you have had this issue in the past, please let me know.

I took about 20 images of different colored sticky notes on a white wall. Each image had anywhere between 5 and 15 sticky notes.

I decided to use ImageAI's custom object detection API, since this was a pretty quick challenge. I didn't want to get stuck in hours of training custom CNNs. ImageAI uses a YOLOv3 architecture. I trained for 100 epochs with scores topping off at 1.0 after 50 epochs.
The documentation can be found here : https://imageai.readthedocs.io/en/latest/customdetection/

This was my first attempt at using OCR, so I wasn't quite sure which API to use. I went with keras-ocr since I am comfortable using that framework. If you have any advice on other algorithms to use please let me know. 
The documentation can be found here : https://github.com/faustomorales/keras-ocr

## Example Output
![Cropped output image](https://github.com/tsugg/Sticky-Notes/blob/master/test_image.JPG)
![Corresponding output text file] (https://github.com/tsugg/Sticky-Notes/blob/master/test_text.JPG)

# INSTRUCTIONS

## Step 1: Download the model 
Download from here: https://drive.google.com/open?id=1waRi2YBuNY6pX7kCYy_kWsI0AylFpYco
(You can also download it from the models directory. You will have to download it form the UI, since the file size becomes an issue when cloning the repository)

## Step 2: Go to the Google Colab Notebook
Download from here : https://drive.google.com/file/d/1Qc1E8z0MPUzzVZIeFxlGACtgFJP2tQH_/view?usp=sharing
and upload it to colab.research.google.com
(You can also open it directly from the master branch)

## Step 3: Follow instructions on the Google Colab notebook

# Conclusion

The object detection part of the challenge seemed to go very well. I wonder how well this would actually perform in a work environment, since I trained on a white wall. I know many of the walls in offices are glass, so that may have an effect on the model mAP. If this actually gets implemented, I hope someone with better handwritting than me is writing on the notes, because the OCR algorithm sure didn't like mine. 
