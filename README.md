#Ennui Alert Emanator

## A Boredom Detector and Alert System using the YOLO algorithm + OpenCV to enhance user productivity and focus through warnings.



Install and configure modules/files:
pipenv shell
install torch torchvision torchaudio
git clone https://github.com/ultralytics/yolov5.git
cd yolov5
pipenv install -r requirements.txt 
touch dataset.yaml
pipenv install Pillow==9.5.0
(Configure dataset.yaml)

python create_images.py (creates training images using OpenCV)
![alt text](https://cascable.se/help/pro-webcam/how-to-look-awesome/macbook-webcam.jpg)




label the created images:
git clone https://github.com/heartexlabs/labelImg.git
cd labelImg
python labelImg.py
(label the images)
![alt text](https://raw.githubusercontent.com/tzutalin/labelImg/master/demo/demo3.jpg)


Train the model:
python train.py --img 640 --epochs 500 --data dataset.yaml --weights yolov5s.pt

![alt text](https://www.researchgate.net/profile/Franck-Luthon/publication/305703907/figure/fig4/AS:1010771270070279@1617998058994/Face-bounding-box-and-landmark-points-detection-using-the-algorithm-in-8.png)

