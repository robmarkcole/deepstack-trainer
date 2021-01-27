# DeepStack Custom Object Detection Training

DeepStack is a cross platform AI engine for performing Object Detection, Face Detection and Face Recognition on the edge and the cloud.

This repo provides functionality to train object detection models on your own objects, the model from this can be instantly deployed
to DeepStack on Desktop devices, Nvidia Jetson devices and the cloud.

Follow the instructions in this repo for setup, preparing your dataset, training your model and deploying for production use with DeepStack.


# Setup and Train on Google Colab

# Local Setup and Installation

## Clone DeepStack Trainer
<pre>
git clone https://github.com/johnolafenwa/deepstack-trainer
</pre>

## Install Requirements
- Install Python3.7 or higher
- Install [PyTorch](https://pytorch.org)
- Run <pre> pip install -r requirements.txt </pre>

## Debugging
- `source venv/bin/activate`
- `python3 detect.py --source "fire-images" --weights fire.pt --conf 0.3 --img-size 460`

```
image 1/7 /Users/robin/Github/deepstack-trainer/fire-images/Heath-fire-1.jpg: 384x480 3 fires, Done. (0.494s)
image 2/7 /Users/robin/Github/deepstack-trainer/fire-images/candle-1.jpg: 352x480 Done. (0.796s)
image 3/7 /Users/robin/Github/deepstack-trainer/fire-images/fire-annotated.jpg: 448x480 1 fires, Done. (0.492s)
image 4/7 /Users/robin/Github/deepstack-trainer/fire-images/fire-car.jpg: 320x480 1 fires, Done. (0.284s)
image 5/7 /Users/robin/Github/deepstack-trainer/fire-images/fire-car2.jpg: 288x480 1 fires, Done. (0.248s)
image 6/7 /Users/robin/Github/deepstack-trainer/fire-images/fire-car3.jpg: 480x480 1 fires, Done. (0.460s)
image 7/7 /Users/robin/Github/deepstack-trainer/fire-images/fire-house.jpg: 384x480 1 fires, Done. (0.671s)
```