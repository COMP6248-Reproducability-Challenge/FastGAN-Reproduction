# FastGAN-Reproduction

## Paper
The original paper is available at [OpenReview](https://openreview.net/forum?id=1Fqg133qRaI)

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

## Team members
* **Ming Cheng** [mc18g20@soton.ac.uk]() 
* **Qianyi Zhang** [qz1u20@soton.ac.uk]() 
* **Shaoyuan Xiao** [sx1n20@sotom.ac.uk]() 
* **Qinglie Zhu** [qz5e20@sotom.ac.uk]() 


*This code is provided under the GNU General Public License v3.0
## License and copyright notice
This code is provided under the GNU General Public License v3.0

## Original Code
The author's code at [Github](https://github.com/odegeasslbc/FastGAN-pytorch)
