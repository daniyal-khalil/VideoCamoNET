# VideoCamoNET
Description of paper:

One of the sophisticated detection tasks in Computer vision is Camouflage Detection regarding which numerous well-performing models were proposed. Since in this task, camouflaged objects should be detected into the wild images and stationary objects we assumed to extend this approach to dynamic cases, involving frames that captures human mobility in CAMO-UOW dataset. For this overview, we considered the COD10K, containing 10k images.  

Codes:

Upload databases which resize the images for the model usage

Resnet code defines a forward resnet architecture

Train_eval describs about the loss function which is applied for both searching and identification modules

SINet comes with combination of the searching module, the identification modules, Receptive fields, and Partial decoder components

Training and test protocols:

The optimum results are obtained on 40-th iteration by considering 0.0001 as learning rate, 36 as the batch size. The size of training image is 352, and gradient decay margin, decay rate of learning rate per decay step are set in 0.5 and 0.1 consecutively. The number of channels is set on 32. The overall evaluation on training is based on comparing research and identification output with Ground Truth which is correlated with the mean absolute error. It approximately takes 60-70 minutes for training.


Dataset:

This dataset was published in 2017 in order to address the issue of camouflaged moving foreground detection in the original scenes. It involves 10 different videos, containing 3,517 video frames in total. The details of each videos are dedicated in the table below. to give a brief introduction about the videos, each ones consists of a person or some people (known as foreground objects) who were similar to the back ground colors. The ground truth manually segmented with pixel based labeling for each frames. In addition, videos were recorded in both indoor and outdoor as well. This dataset is less frequently utilized for benchmarking.
Link: https://datasets.bifrost.ai/info/1843

Daniyal Khalil \
Muhammad Bilal Bin Khalid \
Sepehr Nour Mohammad
