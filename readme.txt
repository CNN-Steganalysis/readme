%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Purpose
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
The purpose of this code is to train or test a residual network with adaptive content suppression for image steganalysis. The implementation is based on the MatConvNet platform. 

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Files
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
run_experiment: this is the main function, which can be used to test a well trained model on the S-UNIWARD steganography at 0.4 bpp, or to learn a new model to detect a given steganographic algorithm.

train_model: the function to train the model.

test_model: the function to test the model.

cnn_steganalysis_setup_data: the function to determine training samples and testing samples. In our implementation, '1' represents the training sample while '2' represents the testing sample.

getBatchFn, getDagNNBatch: the function to read images from specified paths

setup: the function to setup environment for the proposed model

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Folders
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
dependencies: this folder contains basic functions of constructing a CNN model with the MatConvNet platform. It contains two sub-folders, i.e. matconvnet and vlfeat. These files can be downloaded from following links:
vlfeat: http://www.vlfeat.org/
matconvnet: http://www.vlfeat.org/matconvnet/ 

nets: this folder contains a well trained model for S-UNIWARD steganography: trained_net.mat and an untrained model: untrained_net.mat

results: the trained model will be saved in this folder. 
