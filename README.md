# Real-time-video-based-action-recognition

I used motion stream CNN with ResNet50 for modeling video information in UCF101 dataset. I don't have too much time so I trained only 3 actions (**ApplyEyeMakeup, ApplyLipstick, Archery**) with epochs 50 my pretrain model can be download from here.  I choose the Two-Stream CNNs Technique according to [this blogs](https://towardsdatascience.com/deep-learning-architectures-for-action-recognition-83e5061ddf90).





#### Motion CNN

In every mini-batch, generator selected 5 consequence images and stacked  these images.



### Download the preprocessed data directly from

```bash
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.001
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.002
wget http://ftp.tugraz.at/pub/feichtenhofer/tsfusion/data/ucf101_jpegs_256.zip.003

cat ucf101_jpegs_256.zip* > ucf101_jpegs_256.zip
unzip ucf101_jpegs_256.zip
```





## Reference Papers

- [[1\] Two-stream convolutional networks for action recognition in videos](https://arxiv.org/pdf/1406.2199.pdf)
- [[2\] Real-time Action Recognition with Enhanced Motion Vector CNNs](https://arxiv.org/pdf/1604.07669.pdf)
- [[3\] Towards Good Practices for Very Deep Two-Stream ConvNets](https://arxiv.org/pdf/1507.02159.pdf)
