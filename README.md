# Digit Classifier
<code>digitclassifier</code> is a JdeRobot component which captures live video and classifies the digits found in every frame with a convolutional neural network. Implementations in both Keras and Tensorflow are available.
## Usage
In order to test it with Python 2.7 you must install: 
* JdeRobot ([installation guide](http://jderobot.org/Installation))
* OpenCV 3 (it will be automatically installed with JdeRobot)
* Keras ([installation guide](https://keras.io/#installation))
* TensorFlow as Keras Backend ([installation guide](https://www.tensorflow.org/install/install_linux))

If you want to launch <code>digitclassifier</code>, open a terminal and run:
<pre>
cameraserver cameraserver.cfg
</pre>
This command will start <code>cameraserver</code> driver, which will serve video from the webcam. In another terminal, access Keras or TensorFlow folder and run:
<pre>
python digitclassifier.py digitclassifier.yml
</pre>
That command should launch the component and you should see something like this:
![Alt Text](https://media.giphy.com/media/xT0xevE4RgzA4CTEju/giphy.gif)

If you want to train a new model with the augmented MNIST datasets we used for training, here they are:
* [HDF5 datasets](https://mega.nz/#!hV12GapC!3eGRv0Ty8VRoJxhnbrG_4e21QUnPNjraTnqUJog7PxU)
* [LMDB datasets](https://mega.nz/#!NBkBTSRI!TPfLk4nHY5WjconmhbI9jV_yZLvnImDzextQSBcA6Wk)

More info about Keras implementation: [http://jderobot.org/Dpascual-tfg]

More info about TensorFlow implementation: [http://jderobot.org/Naxvm-tfg]
