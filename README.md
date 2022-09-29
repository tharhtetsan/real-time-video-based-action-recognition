# Real-time-video-based-action-recognition

I used motion stream CNN with ResNet101 for modeling video information in UCF101 dataset. I don't have too much time so I trained only 4 actions (**"Archery","ApplyEyeMakeup","BaseballPitch","Basketball**) with only epochs 50 and my pretrain model can be download from [here](https://drive.google.com/file/d/13hGC5hBJ9T1uUCBmMwJYcgFVQL7eQC8w/view?usp=sharing).  I choose the Two-Stream CNNs Technique according to [this blogs](https://towardsdatascience.com/deep-learning-architectures-for-action-recognition-83e5061ddf90).





#### Result

![](output_result_gif.gif)





#### Motion CNN

In every mini-batch, generator selected 5 consequence images and stacked  these images. 


### Download the dataset

- ##### download from the original [UCF101](https://www.crcv.ucf.edu/data/UCF101.php)

- ##### Or the preprocessed data directly from

```bash
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.001
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.002
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.003
```





## Reference Papers

- [[1\] Two-stream convolutional networks for action recognition in videos](https://arxiv.org/pdf/1406.2199.pdf)
- [[2\] Real-time Action Recognition with Enhanced Motion Vector CNNs](https://arxiv.org/pdf/1604.07669.pdf)
- [[3\] Towards Good Practices for Very Deep Two-Stream ConvNets](https://arxiv.org/pdf/1507.02159.pdf)
