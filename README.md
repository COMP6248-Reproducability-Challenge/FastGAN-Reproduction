# FastGAN-Reproduction

## Original Paper
The original paper is available at [OpenReview](https://openreview.net/forum?id=1Fqg133qRaI)

## Data
The datasets used in the original paper can be found at [link](https://drive.google.com/file/d/1aAJCZbXNHyraJ6Mi13dSbe7pTyfPXha0/view?usp=sharing). 


## How to Run
Place all your training images in a folder, and simply call
```
python train.py --path /path/to/RGB-image-folder
```
You can also see all the training options by:
```
python train.py --help
```
The code will automatically create a new folder (you have to specify the name of the folder using --name option) to store the trained checkpoints and intermediate synthesis results.
Once finish training, you can generate 100 images (or as many as you want) by:
```
cd ./train_results/name_of_your_training/
python eval.py --n_sample 100 
```

```
cd /path/to/benchmarking
python fid.py --path_a /path/to/RGB-image-folder  --path_b /path/to/main
```
The code will compute  Frechet Inception Distance (FID) for origional image and generated image

```
cd /path/to/scripts
python find_nearest_neighbor.py
```
This code will find the closest real-image for generated images and output the pair of origional image and generated image


## Pre-trained models
This [Dog class parameters](https://drive.google.com/drive/folders/1hReq_bFW-2xU8FmOfE78YQBko6aNV-25) shared two pre-trained models: image size = 1024, batch size = 8 and image size =256,batch size = 8. 

This [Cat class parameters](https://drive.google.com/drive/folders/1QEvdZlQhHZAenWyvVrESjKPQNGQT5SHN?usp=sharing) shared two pre-trained models: image size = 512, batch size = 2 and image size =256,batch size = 8.



## Team members
* **Ming Cheng** [mc18g20@soton.ac.uk]() 
* **Qianyi Zhang** [qz1u20@soton.ac.uk]() 
* **Shaoyuan Xiao** [sx1n20@sotom.ac.uk]() 
* **Qinglie Zhu** [qz5e20@sotom.ac.uk]() 


## License and copyright notice
This code is provided under the GNU General Public License v3.0

## The report
You can see the report at [Link](https://sotonac-my.sharepoint.com/:b:/r/personal/qz5e20_soton_ac_uk/Documents/Report.pdf?csf=1&web=1&e=btZtm6)

## Original Code
The author's code at [Github](https://github.com/odegeasslbc/FastGAN-pytorch)
