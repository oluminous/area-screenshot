## Create a screenshot by clicking the edges of the area you want to capture.

## Requirements
  - Python 3.3+
  - [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/index.html)    ```pip install pyautogui```
  - [Pynput](https://pynput.readthedocs.io/en/latest/#)     ```pip install pynput```
  
    On Linux, ```pyautogui``` has some extra dependencies. Simply run the following commands from the terminal to install them:
    ```sudo pip3 install python3-xlib```, 
    ```sudo apt-get install scrot```, 
    ```sudo apt-get install python3-tk```, and 
    ```sudo apt-get install python3-dev``` 
  
## How to Use
  1. After installing the required packages, simply run the script from the folder you want the screenshot to be saved.
  2. Once the script starts, your terminal will minimize automatically, so as to allow you select the area you want to capture without obstruction. On the terminal itself, it's simply ```print``` statements that are executing.
  3. **Click** the edges of the area in the following order: top-left, top-right, bottom-left, bottom-right. (Note that it's not a bounding box--there's no dragging; but only _clicking_ of the edges of the intended image)
  4. After clicking the bottom-right, your terminal returns automatically with a message confirming the successful creation of the screenshot.
  5. The screenshot itself would be found in the folder you invoked the script from with a '```.png```' extension.

## Example
![](usage.gif)
  
  
### Motivation
This project is a prerequisite to another I'm currently working on that deals with text extraction from images. I have an app on my phone (FooView) that allows me draw a boundary box around an image or a video or anything really, and then it extracts text from the resulting image almost immediately. I usually do this a lot for links embedded in images. I'll then easily paste the generated text in my browser and go. A demo can be seen [here](https://twitter.com/_Olums/status/1066411959950692353).

I have no app that does this on my laptop so I'm creating one for my use.The steps are simple: select an area with text I want to extract, create an image, then extract the text using Optical Character Recognition. This repo is just stage one.

All the other python screenshot libraries/scripts I saw dealt solely with creating select images using coordinates. I wanted one where I could manually create the area screenshot without knowing the coordinates. 



