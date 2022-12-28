Hello this is Syed Anwar.

This is the task assigned to me by the Governament Innovation Lab(GIL) Quetta Pakistan. The task is to take any dataset from kaggle (enywhere) and train a VGG19 or Inception model.

I decided to take the Cats_vs_Dog Dataset (http://www.kaggle.com/c/dogs-vs-cats/data) from kaggle and I read all the related work. So I Noticed that the model highest accuracy was gain in 2013 is 97% with complete dataset. I Decided to use less than 10% data to beat the challenge and then I splitt the data into 3 parts. 

I take 2000 data for training 1000 for validation and 1000 for testing from the 25000 image dataset. after prerpocessing dataset and using data augumentation technique I train model and i get 96% training accuracy 95% validation and 95% testing accuracy.

After training the and evaluated the model. I saved the model "vgg19.model" and also in HDF5 format "my_model.hf".

In deploy_raspberrypi directory these is a python file named "vgg19_raspberryPi.py" for running this program on raspberrypi you need to do two things:
1: Install any Operating System on your SSD card and put it in the raspberrypi.
2: Install the dependencies:
	2.1: You must need to install following packages on raspberrypi:
		1: OpenCv (cv2)
		2: TensorFlow
		3: Numpy
		4: Keras (will be inside TensorFlow by default)
		
