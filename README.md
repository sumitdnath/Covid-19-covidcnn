# 🛑 Note: This model is still not reliable to use. It is just a research for now. 

To read Motivation and Goal behind this research go to this [Github Repository](https://github.com/ieee8023/covid-chestxray-dataset/blob/master/README.md).
# Dataset 
```
dataset
├── test
│   ├── covid19 [32 entries]
│   ├── normal [25 entries]
│   └── pneumonia [20 entries]
├── train
│   ├── covid19 [219 entries]
│   ├── normal [210 entries]
│   └── pneumonia [210 entries]
└── validate
    ├── covid19 [32 entries]
    ├── normal [20 entries]
    └── pneumonia [20 entries]
```

# Model Design
![model_161](model/images/Covidcnn_161.svg)


# Model Result
![Model Accuracy](model/images/modelAccuracy_100.png)
![Model Loss](model/images/modelLoss_100.png)

* This model was trained on **very small sets of images**, therfore the model is not **generalized** enough to use. 

# Deploying model
After the model was trained it was compressed into [tflite](https://www.tensorflow.org/lite/) model. After which it was 
deployed on [flutter](https://flutter.dev/) application.
## ScreenShots of Flutter application
<img src="https://github.com/Thehunk1206/Covid-19-chest-X-ray/blob/master/Application/Application%20Screenshot/Screenshot_20200413-200009.png" alt="ss"
width="200" height="400"/>
<img src="https://github.com/Thehunk1206/Covid-19-chest-X-ray/blob/master/Application/Application%20Screenshot/Screenshot_20200413-200028.png" alt="ss"
width="200" height="400"/>
<img src="https://github.com/Thehunk1206/Covid-19-chest-X-ray/blob/master/Application/Application%20Screenshot/Screenshot_20200413-200120.png" alt="ss"
width="200" height="400"/>

# Dataset source 
- [Covid19](https://github.com/ieee8023/covid-chestxray-dataset).
- [pnemonia and normal X-ray](https://data.mendeley.com/datasets/rscbjbr9sj/2)


This repository will be updating as the dataset will grow more and more.
Any contribution would be appreciated.

**more detailed documentation comming soon**


# Citation

Paper availabe [here](https://arxiv.org/abs/2003.11597)


```
@article{cohen2020covid,
  title={COVID-19 image data collection},
  author={Joseph Paul Cohen and Paul Morrison and Lan Dao},
  journal={arXiv 2003.11597},
  url={https://github.com/ieee8023/covid-chestxray-dataset},
  year={2020}
}
```


