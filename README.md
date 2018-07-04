# FaceRecognition

* Face recognition program using pyton , tensorflow and inception CNN.

* Setup

  
      pip install tensorflow
      pip install opencv-python
     
      
* Converting Images
    keep both video file and frame.py in same folder. Use 'video.mp4' as a name of video input.

    python -m scripts.frame


* (Re)Training

  To train the model:
  
      python -m scripts.retrain \
      --output_graph=DataSet/retrained_graph.pb \
      --output_labels=DataSet/retrained_labels.txt \
      --architecture=inception_v3 \
      --image_dir=DataSet/images

* Using the Model

  To recognize:
    For single label classification
      python -m scripts.singleLabel
    For multi label classification 
      python -m scripts.multiLabel

* Created By: Deep Parmar ('deep56parmar@hotmail.com')