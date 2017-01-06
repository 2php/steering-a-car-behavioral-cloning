# Steering a car

Here is behavioral cloning project, that I did as part of [Udacity Self-Driving Car Nanodegree](https://www.udacity.com/drive). Behavioral cloning is technics for teaching neural networks to do useful things or behave in desired way. In this example we need to steer a car while driving in simulator ([Linux](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f0f7_simulator-linux/simulator-linux.zip), [MacOS](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f290_simulator-macos/simulator-macos.zip), [Win32](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f4b6_simulator-windows-32/simulator-windows-32.zip), [Win64](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f3a4_simulator-windows-64/simulator-windows-64.zip)) based onboard camera images. So firstly we need to drive the car ourselves and collect the images from the camera and corresponding steering wheel angle positions. Then we need to teach neural network to return steering angle for provided image - well known and tested supervised learning task. Sounds pretty simple. Let's see my particular version of it.
There is nice [Nvidia paper](http://images.nvidia.com/content/tegra/automotive/images/2016/solutions/pdf/end-to-end-dl-using-px.pdf) where they applied this approach to drive a real car. You may find videos of it on youtube. It's pretty amazing to watch. I use the same but simplified method. Since we are working with images we need [convolutional neural network](https://en.wikipedia.org/wiki/Convolutional_neural_network) or CNN. There are a lot of free tutorials over the internet about CNNs. [For example](https://www.udacity.com/course/deep-learning--ud730). So I decided to use similar to Nvidia CNN.

![CNN architecture](https://github.com/parilo/steering-a-car-behavioral-cloning/blob/master/Proj3-CNN.png "CNN architecture")
