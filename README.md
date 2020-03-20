# COVID-19
CNN model that diagnoses using Chest X-ray medical images

**DISCLAIMER: This model was designed and implemented for educational purposes. it MUST NOT be used for medical diagnosis as it was NOT tested by a field expert.**

## Introduction:
CoVID19 is a disease caused by the newly identified virus SARS-CoV-2 of the Corona Viruses family<sup>1</sup>. The disease's incubation period is 14 days, with most cases being between 4-5 days<sup>2</sup>. The clinical presentation starts with coughing, fever, dyspnea, and bilateral infiltrates on chest imaging. The presentation can be severe in a lot of cases, especially in old people<sup>3</sup>. 
Radiological features on chest x-ray of confirmed COVID-19 cases were parenchymal abnormalities, specifically peripheral consolidations (accumulation of fluids)<sup>4</sup>; although Chest X-rays weren't so inclusive.


1.  World Health Organization. Director-General's remarks at the media briefing on 2019-nCoV on 11 February 2020. [Here](https://www.who.int/dg/speeches/detail/who-director-general-s-remarks-at-the-media-briefing-on-2019-ncov-on-11-february-2020)
2.  Li Q, Guan X, Wu P, Wang X, Zhou L, Tong Y, et al. Early Transmission Dynamics in Wuhan, China, of Novel Coronavirus–Infected Pneumonia. New England Journal of Medicine. 2020Jan29;
3.  Wu Z, Mcgoogan JM. Characteristics of and Important Lessons From the Coronavirus Disease 2019 (COVID-19) Outbreak in China. Jama. 2020Jan24;
4.  Yoon SH, Lee KH, Kim JY, Lee YK, Ko H, Kim KH, et al. Chest Radiographic and CT Findings of the 2019 Novel Coronavirus Disease (COVID-19): Analysis of Nine Patients Treated in Korea. Korean Journal of Radiology. 2020Jan26;21(4):494.

*I would like to thank Dr.[Mohammed](https://github.com/mrg0lden) for helping me understand this disease and participating in this paragraph*

## Dataset:

1. The posstive cases of COVID-19 X-ray images taken from Dr. Cohen in his 
[repo](https://github.com/ieee8023/covid-chestxray-dataset)
2. The normal cases taken from dataset that's published in Kaggle's dataset 
[Here](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia/data#).


## Model:

I designed 2 different models of CNN, one of them contains 4 layers with padding and `relu` as an activation function after every 2 layers there is a `max-pooling` layer, then two fully connected layers with `relu` and `softmax` as an activation function. the second one contains 2 Convolution layers with `relu` as an activation function follows by the `max-pooling` layer. The optimizer for both models is `Adam` and `binary_crossentropy` as a loss function. 

## Result & Predection 
The accuracy for both models is above 95% on the validation set.
1st Model and 2ed Model: 
![](https://github.com/HebahAlshamlan/Covid-19/blob/master/img/Model2.png)
![](https://github.com/HebahAlshamlan/Covid-19/blob/master/img/Model1.png)

* Predection using 2nd model:
![](https://github.com/HebahAlshamlan/Covid-19/blob/master/img/Covid-19%2B.png)
![](https://github.com/HebahAlshamlan/Covid-19/blob/master/img/Covid-19-.png)
## To Do:
- [ ] Testing the model.
- [ ] Calculate the confusion matrix.
- [ ] Try on CT scan imeages.
- [ ] Try ResNet model on this problem.


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
