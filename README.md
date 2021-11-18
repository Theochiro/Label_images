# Label_images
First, download the images from here:

```bash
https://drive.google.com/file/d/1c5gTxBfUvL-VWkZq_PTlxKZLaBVFZceE/view?usp=sharing
```

Second, install [LabelImg](https://github.com/tzutalin/labelImgl) and run the following commands:

```bash
cd ~/
mkdir images
mkdir labels
```
Then copy the contents of the drive images into the image folder. Then create the following file:

```bash
cd labels
gedit classes.txt
```
Then copy and paste this into the new file and into ```~/labelImg/data/predefined_classes.txt```:
```bash
painting1
painting2
painting3
painting4
```
Then run the following command to start labeling :) 
```bash
cd ~/labelImg
python3 labelImg.py 
```
Select the appropriate directory to save the image labels and change the labeling form from PASCAL/VOC to YOLO.
Make sure to delete each image which does not contain any label using ```Shift+Ctrl+D```
Draw a bounding box with the ```W``` shortcut.
Move around images using ```A```  and ```D``` .
Save using ```Ctrl+S``` 
