# dog_project
This is a project from Udacity's Deep Learning Nanodegree (Convolutional Neural Networks module).

## Datasets
* [Dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip) (unzip the folder and place it in the repo, at location `path/to/dog_project/dogImages`)
* [Human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip) (unzip the folder and place it in the repo, at location `path/to/dog_project/lfw`)
* [VGG-16 bottleneck features for the dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) (place it in the repo, at location `path/to/dog_project/bottleneck_features`)

## Environment
If you plan to install TensorFlow with GPU support on your local machine, follow [this guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.

Use the following commands to create (and activate) the new environment:

* **Linux** (to install with GPU support, change `requirements/dog-linux.yml` to `requirements/dog-linux-gpu.yml`): 
	
  ```
	conda env create -f requirements/dog-linux.yml
	source activate dog-project
  ```

* **Mac** (to install with GPU support, change `requirements/dog-mac.yml` to `requirements/dog-mac-gpu.yml`): 
	
  ```
	conda env create -f requirements/dog-mac.yml
	source activate dog-project
  ```
  
**Note:** Some Mac users may need to install a different version of OpenCV
	
  ```
	conda install --channel https://conda.anaconda.org/menpo opencv3
  ```

* **Windows** (to install with GPU support, change `requirements/dog-windows.yml` to `requirements/dog-windows-gpu.yml`):
  
  ```
	conda env create -f requirements/dog-windows.yml
	activate dog-project
	```
  
## Backend
Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
* **Linux** or **Mac**:

  ```
  KERAS_BACKEND=tensorflow python -c "from keras import backend"
	```
    
* **Windows**:
 
  ```
	set KERAS_BACKEND=tensorflow
	python -c "from keras import backend"
	```
