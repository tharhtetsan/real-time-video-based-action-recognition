# Real-time-video-based-action-recognition

I used motion stream CNN with ResNet101 for modeling video information in UCF101 dataset. I don't have too much time so I trained only 4 actions (**"Archery","ApplyEyeMakeup","BaseballPitch","Basketball**) with only epochs 50 and my pretrain model can be download from [here](https://drive.google.com/file/d/13hGC5hBJ9T1uUCBmMwJYcgFVQL7eQC8w/view?usp=sharing).  I choose the Two-Stream CNNs Technique according to [this blogs](https://towardsdatascience.com/deep-learning-architectures-for-action-recognition-83e5061ddf90).





#### Result

![](output_result_gif.gif)





#### Motion CNN

In every mini-batch, generator selected 5 consequence images and stacked  these images. How to Run the Code

##### 

#### How to train the model with own data

- ##### download from the original [UCF101](https://www.crcv.ucf.edu/data/UCF101.php)

- ##### Or the preprocessed data directly from

```bash
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.001
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.002
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.003
```

- update data path in **[model_train_v1.ipynb](https://github.com/tharhtetsan/real-time-video-based-action-recognition/blob/c01958f5c11d62be99078e12e62d3ed4a2070ace/model_train_v1.ipynb)**



#### How to test the model

- download the [trained model.](https://drive.google.com/file/d/13hGC5hBJ9T1uUCBmMwJYcgFVQL7eQC8w/view?usp=sharing)

- update model path and in video path in **[model_predict.ipynb](https://github.com/tharhtetsan/real-time-video-based-action-recognition/blob/c01958f5c11d62be99078e12e62d3ed4a2070ace/model_predict.ipynb)**





## Reference Papers

- [[1\] Two-stream convolutional networks for action recognition in videos](https://arxiv.org/pdf/1406.2199.pdf)
- [[2\] Real-time Action Recognition with Enhanced Motion Vector CNNs](https://arxiv.org/pdf/1604.07669.pdf)
- [[3\] Towards Good Practices for Very Deep Two-Stream ConvNets](https://arxiv.org/pdf/1507.02159.pdf)



