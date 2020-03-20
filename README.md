# Covid-19
CNN model for diagnosis from X-ray image 

**DISCLAIMER: This model was designed and implemented for educational purposes. it MUST NOT be used for medical diagnosis as it was NOT tested by a field expert.**

## Introdiction:


## Dataset:

1. The posstive cases of COVID-19 X-ray images I take them from Dr. Cohen in his 
[repo](https://github.com/ieee8023/covid-chestxray-dataset)
2. The normal cases I take them from dataset that published in Kaggle's dataset 
[Here](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia/data#).


## Model:

Designed 2 different models of CNN, one of them contains 4 layers with padding and `relu` as an activation function after every 2 layers there is a `max-pooling` layer, then two fully connected layers with `relu` and `softmax` as an activation function. the second one contains 2 Convolution layers with `relu` as an activation function follows by the `max-pooling` layer. The optimizer for both models is `Adam` and `binary_crossentropy` as a loss function. 

## Result & Predection 
The accuresy for both models is apove 95% accurce on the valudation set. 


## To Do:
- [ ] Testing the model.
- [ ] Calculate the confusion matrix.
- [ ] Try on CT scan imeages.
- [ ] Try ResNet model on this problem.


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
