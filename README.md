APCGAN-AttuNet


## Data:

The image folder contains all the data utilized in this part. In the images floder, there contains three sub-floders: 


| subfolders      | info                                           |   training | 
| :------------:   | :-------------:                                  |:--------:|
| cracks          | 587 original images from [DeepCrack](https://github.com/yhlleo/DeepCrack)| 300 from [DeepCrack](https://github.com/yhlleo/DeepCrack)|
| cracks-tradition| traditional augmentation   |300 from [DeepCrack](https://github.com/yhlleo/DeepCrack) + real-like images from traditional augmentation |
| cracks-DCGAN     |   DCGAN     |300 from [DeepCrack](https://github.com/yhlleo/DeepCrack) + real-like images from DCGAN |
| cracks-APC-GAN|    APC-GAN    | 300  from [DeepCrack](https://github.com/yhlleo/DeepCrack) + real-like images + APCGAN    |      

The **testing data** are all from the DeepCrack which contains **287** crack images.
## Models:
All the models are in the model file.

AttuNet




## Run Order:
### First, setup the environment on your PC.
 Create the environment in your terminal: 
```python 
conda env create -f environment.yml 
```
You can also update an environment to make sure it meets the current requirements in a file:
```python 
conda env update -f environment.yml
```
### Second, augment the images amount.

In augmentation folder: 

random_crop.py : random crop is used as a traditional image augmentation method and the images produced will be stored in augmentation/results/random_crop

DCGAN.py : use DCGAN method to generate real-like images which will be stored in augmentation/results/DCGAN

APCGAN.ipynb : use DCGAN method to generate real-like images which will be stored in augmentation/results/APCGAN

After get the generated images, annotate these images 

### Third, 


3. Deep Learning:

3.1 AttuNet

3.2 AttuNet-min

3.3 U-Net

3.4 
