[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"

# Dog-breed-classifier
Predict dog breed using Convolutional Neural Networks (CNN).  This project is part of the Udacity Deep Learning Nanodegree.

# Introduction
In this project, we'll how to build a pipeline to process real-world, user-supplied images. Given an image of a dog, your algorithm will identify an estimate of the canine's breed. If supplied an image of a human face, the code will identify the resembling dog breed. 

![Sample Output][image1]

# Instructions

1. Set up the Jupyter ipython notebook environment
2. Load and prepare the data using pytorch
3. Use VGG-16 pretained model to test the data
4. Build, train and test the CNN from scratch
5. Build, train and test the CNN using Tranfer Learning
6. Train the network using training and validation dataset
7. Test the network for accuracy using test dataset

## 1. Set up the Jupyter ipython notebook environment
## 1.1 Installation

Download Anaconda

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Windows-x86_64.exe
[win32]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Windows-x86.exe
[mac64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-MacOSX-x86_64.sh
[lin64]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86_64.sh
[lin32]: https://repo.anaconda.com/archive/Anaconda3-2018.12-Linux-x86.sh

**Install** [Anaconda](https://docs.anaconda.com/anaconda/install/) on your machine. 

## 1.2 Create and Activate the Environment

Please go though this [doc](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) before you creating an environment.
After that create a environment using following command:

```
conda create --name deep-learning
```

Then activate the environment using following command:

```
activate deep-learning
```

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

**Now, you can create a local version of the project**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/sureshsubr/dog-breed-classifier.git
cd dog-breed-classifier
```

2. Install PyTorch and torchvision; this should install the latest version of PyTorch.
	
	- __Linux__ or __Mac__: 
	```
	conda install pytorch torchvision -c pytorch 
	```
	- __Windows__: 
	```
	conda install pytorch -c pytorch
	pip install torchvision
	```

3. Install a few required pip packages, which are specified in the requirements text file.
```
pip install -r requirements.txt
```
Or
```
conda install --yes --file requirements.txt
```

4. That's it! Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
```
jupyter notebook
```

Once jupyter notebook instance is open follow the remaining instructions steps #2 - #7 in the ipython notebook called `dog_app.ipynb`.

To exit the environment when you have completed your work session, simply close the terminal window.

__NOTE:__ In the notebook, you will need to train CNNs in PyTorch.  If your CNN is taking too long to train, feel free to pursue the options under the section __Accelerating the Training Process__ below.



#### (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen CNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own, for example, you can use Amazon Web Services to launch an EC2 GPU instance but note that this costs money!!

