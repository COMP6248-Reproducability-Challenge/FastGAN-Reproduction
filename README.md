# FastGAN-Reproduction

## Paper
The original paper is available at [OpenReview](https://openreview.net/forum?id=1Fqg133qRaI)

##How to RUn
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

## Authors


## Team members
* **Ming Cheng** [mc18g20@soton.ac.uk]() ID：31559395 
* **Qianyi Zhang** [qz1u20@soton.ac.uk]() ID：30931274 
* **Shaoyuan Xiao** [sx1n20@sotom.ac.uk]() ID：32315198 
* **Qinglie Zhu** [qz5e20@sotom.ac.uk]() ID：332453566  


*This code is provided under the GNU General Public License v3.0
## License and copyright notice
This code is provided under the GNU General Public License v3.0
