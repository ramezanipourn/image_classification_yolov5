# image_classification_yolov5

<details>
<summary>Install</summary>
<br>
1.Clone repo and install requirements.txt
        
* git clone https://github.com/ultralytics/yolov5  # clone
* cd yolov5
* pip install -r requirements.txt  # install
</details>



<details>
<summary>inference</summary>
<br>


* You can run Inference with YOLOv5 and PyTorch Hub . Models download automatically from the latest YOLOv5 release.

  import torch

  ## Model
  model = torch.hub.load('ultralytics/yolov5', 'yolov5s')  # or yolov5m, yolov5l, yolov5x, custom

  ## Images
  img = '/content/811755456_b3ac7f05e9.jpg'  # or file, Path, PIL, OpenCV, numpy, list

  ## Inference
  results = model(img)

  ## Results
  results.print()  # or .show(), .save(), .crop(), .pandas(), etc.


* also you can run inference using detect.py and you must put your file link insted of 0:

python detect.py --source 0  # webcam
                          img.jpg  # image
                          vid.mp4  # video
                          path/  # directory
                          path/*.jpg  # glob
                          'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
                          
                          
                          
</details>


<details>
<summary>train</summary>
<br>
        
<details>
