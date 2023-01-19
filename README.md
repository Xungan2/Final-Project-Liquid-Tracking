# Final-Project-Liquid-Tracking
The link to our report: .

In this task, our work can be divided into about three parts.  
First, design a basic model. Second, improve the performance of the basic model. Third, try to use the MOT method to improve the performance of the model.  Here, we will introduce the code framework used in the three parts.  
We use *colab* for this task, so all the codes are in *ipynb* format.
## Part1 - Basic model
We use *YOLO* model under *mmdetection* framework for training. The specific model configuration file is called *yolov3_d53_mstrain-416_273e_coco.py*.  
Here is a link to mmdetection: https://github.com/open-mmlab/mmdetection.  
We haven't saved the trained model here, only the test results.  
The training code is saved in *basic_train.ipynb*.
## Part2 - Improvements
We use two methods to improve the performance of the basic model.  
First, we try to pretrain the *YOLO* model on *Trans10k* dataset.  
Second, we try to scale the test image to different scales, and then integrate all the results as the final result.  
Here we present a table shows all the results.  
![avatar](./table1.png)  
The code is saved in *improvement.ipynb*.
## Part3 - Attempts to use MOT method
To take advantage of the connection between the video frames, we try to use MOT method to improve the model's performance.  
