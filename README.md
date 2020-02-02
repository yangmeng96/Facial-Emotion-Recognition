# Project: Facial Emotion Recognition by Linear Discriminant Analysis
<img src="figs/CE.jpg" alt="Compound Emotions" width="500"/>
(Image source: https://www.pnas.org/content/111/15/E1454)

### [Full Project Description](doc/project3_desc.md)

Term: Fall 2019

+ Team 8
+ Team members
	+ Longo, Stefano sl4444@columbia.edu
	+ Meng, Yang ym2696@columbia.edu
	+ Ruan, Qiuyu qr2127@columbia.edu
	+ Schleicher, Tim trs2145@columbia.edu
	+ Zhao, Nuanjun nz2295@columbia.edu

+ Project summary: In this project, we created a classification engine for facial emotion recognition. After testing a variety of different models, we verified that using LDA with a PCA-driven dimensional reduction offered the best improvement over the baseline model of gradient boosting machines. We achieved 51.2% prediction accuracy with 0.230s and 0.057s training and test feature construction time, 10.953s model training time, 0.004s model testing time.

### [Project Report](doc/main.pdf)
	
**Contribution statement**: 

Yang Meng: Team leader - selected features to overcome the collinearity by deleting duplicated fiducial points and horizontal distances; tuned the number of principle components by cross validation; reduced dimension by PCA to overcome overfitting and applied linear discriminant analysis to selected principle components; measured the time and accuracy as needed; explored a two layer model by SVM as the second layer to reclassify misclassified data given by LDA; explored a boosting method with LDA as weak learners; made some proofs for the feature selection part and explained the pros and cons of our model in the pdf report

Stefano Longo: Focused on the variable selection methods, including best subsets, forward and random forest. Coordinated team efforts and cleaned the GitHub repository.

Nuanjun Zhao: Other models tried including svm and adaboost method with lower accuracy and participation in codes of adaboost combined with LDA by hand which finally failed; Report part in main.pdf. How to reduce the dimension of the duplicated features.

Tim Schleicher: Developed and implemented a Convolutional Neural Network. This included all relevant steps in deep learning such as data processing, model construction and model tuning. The best CNN proved less useful than other models since the amount of data was comparatively limited. He also conceptualized and prepared the presentation.

Qiuyu Ruan: Other models tried including xgboost method with lower accuracy; baseline model: gbm; participation in codes of adaboost combined with LDA by hand which finally failed; Report part in main.pdf. How to reduce the dimension of the duplicated features.


Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
