# adversarial
adversial attacks: robutness of the classification
# Abstract

The advancements in data collection and computing power have led to use neural networks and
deep learning as solutions to solve complex problems. These methods seek to teach computers how
to perform tasks form experience and knowledge instead of explicitly programing them to perform a
task. Therefore, it is more important to ensure the security and robustness of the above-mentioned
algorithms. Recently, the security vulnerability of Deep learning algorithms to adversarial samples has
been extensively recognized as security concern for the reason that the fabricated samples can cause
numerous misbehaviors in the deep learning models while being seen as harmless by humans. This
paper demonstrates how we used adversarial training to enhance the robustness of our models. The
idea is we are going to use two adversarial attacks on the images in our dataset to cause deliberately
incorrect predictions or make the model unable to classify them correctly and then we will implement
methods to robust the neural network.


# Intoduction

Adversarial samples are the current threat to the ex-
isting DL Algorithms and that is because of the per-
turbations they make can cause the model to make

a wrong prediction with a high confidence. Thus,
this phenomenon is considered to be a significant
obstacle to the mass deployment of DL models in
production.

# Dataset
The dataset that we choose to work with for this

study is the GTSRB (German Traffic sign Recogni-
tion Benchmark). It has about 50000 images classi-
fied in 43 classes.

Plot of the GTSRB dataset

# Method and Experiment
Convolutional neural network

To classify our images, we are going to employ con-
volution neural network, also know as CNN or Con-
vNet via keras and tensorflow libraries, with the fol-
lowing architecture:

Conv2D + MaxPool2D + BatchNormalization)
+ activation=’relu’ + activation=’softmax’, with a
loss function “ loss=”categoricalcrossentropy”.
