# Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch
Training the Faster R-CNN neural network to detect objects present in images.

[Dataset used in this project can be downloaded here](https://www.kaggle.com/sixhky/open-images-bus-trucks/activity)

some of the result images



![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/saved%20images%20new1.png)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/sv%206.jpg)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/res_img%201.png?raw=true)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/res_img%203.png?raw=true)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/res_img%200.png?raw=true)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/sv%205.jpg)
![alt_text](https://github.com/PraveenRaja42/Object-Detection-with-FasterRCNN-on-a-Custom-Datasets-using-PyTorch/blob/main/saved%20images/saved%20image3.png)



model training

```
python train_model.py --img_dir [path to image dir] --df_dr [path to meta data (labels, bounding_boxes) dir] --cuda --n_epochs --r [name of the run for tensorboard logging]
```

[trained model weights can be downloaded here](https://drive.google.com/file/d/1-4Hz8-ZQEAFmMDoou8TnY2Y6RAHTo0DX/view?usp=sharing)

model evaluation

```
python model_evaluate.py --serialized_file [path to saved model weights] --img_dir [path to test image dir] --save_path [dir to save result images]
```


```
python evaluate.py --serialized_file [path to saved model weights] --img_dir [path to image dir] --df_dir [path to meta data] --save_dir [dir to save images]
```

tensorboardX installation

```
pip install tensorboardX
```
