## Goal of Notebook
Tujuan dari notebook ini untuk mengetahui dan memprediksi faktor-faktor apa saja (13 faktor independen) yang kuat dalam penyakit jantung koroner(Target faktor dependen)





## Business Problem
Penyakit jantung merupakan salah satu jenis penyakit yang mematikan yang penanganannya harus diatasi sesegera mungkin karena bisa terjadi secara mendadak kepada penderitanya sejak dini sehingga risiko kemungkinan terjadi serangan mendadak kepada penderitanya. Faktor2 penyakit jantung dapat dikenali berdasarkan kondisi tubuh seseorang penderitanya sejak dini sehingga risiko kemungkinan terjadi serangan mendadak dapat diminimalisir dengan berbagai cara, misalnya pola hidup sehat dan olahraga teratur. kondisi kesehatan pada jantung dapat diketahui berdasarkan diagnosis dari dokter. Tujuan dari notebook ini untuk mengetahui faktor-faktor apa saja (13 faktor) yang kuat dalam penyakit jantung koroner

##Matrics
Metrik pada kasus ini adalah diagnosis yang terkena jantung

## Source Dataset
For kaggle https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset

##Attribute Information:
The inputs (variable X/ independent variable) are as follows:
- age:age in years
- sex: 1.male ; 0.female
- (cp) chest pain type (4 values):(0.typical angina ; 1.atypical angina ; 2.non-anginal pain ; 3. asymptomatic)
- chol: serum cholestoral in mg/dl
- fbs:fasting blood sugar > 120 mg/dl(1.true ; 0.false)
- fasting blood sugar > 120 mg/dl
- resting electrocardiographic results (values 0,1,2)
- maximum heart rate achieved
- exercise induced angina
- oldpeak = ST depression induced by exercise relative to rest
- the slope of the peak exercise ST segment
- number of major vessels (0-3) colored by flourosopy
- thal: 0 = normal; 1 = fixed defect; 2 = reversable defect

The output (target/Y/dependent variable) is as follow:
- Target

Conclusion

[ ]
#Create Accuracy Comparison Model
compare = pd.DataFrame({'Model': ['Logistic Regression', 'K-Nearest Neighbour', 'Support Vector Machine',
                                  'Gaussian Naive Bayes', 'Decision Tree', 'Random Forest'
                                  ],
                        'Accuracy': [LRAcc*100, KNNAcc*100, SVMAcc*100, GNBAcc*100, DTCAcc*100, RFAcc*100,
                                     ]})

#Create Accuracy Comparison Model
compare.sort_values(by='Accuracy', ascending=Fals

Setelah menggunakan 6 model Machine Learning. Didapatkan,dari 6 hasil akurasi model Machine Learning didapatkan akurasi model paling tinggi yaitu K-Nearst Neighbour dengan nilai akurasi 86.440678

