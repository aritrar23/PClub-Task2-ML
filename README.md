# PClub-Task2-ML

a) I first googled the problem statement and found several research articles from various reputed websites and journals, like researchgate and ncbi, but their datasets were not publicly available. Then I found this dataset on Kaggle (https://www.kaggle.com/datasets/radhakrishna4/lung-capacity). In the model you can see I plotted various graphs to see if this dataset is correct - and found general trends are beiing followed - like with increasing height/weight, the lung capacity also increases. As for sufficiency, I found that this dataset does not cover people with age > 20, but I had no better option so I had to go with it.

b) I have explained this part in the Jupyter Notebook as well. First I categorized the binary columns(gender, smoke,etc.) and standardized the continuous columns (age, weight). Next I fitted a deep learning Tensorflow neural network with 4 layers. Then I tried a NN with 3 layers. After that I dropped the 'Caesarean' column (since during data analysis I did not find it to be very useful with regards to predicting LungCap) and implement both the 4-layer & 3-layer NN. I found that the 4-layer model with 'Caesarean' column included performed best. Next I tried out various values of lambda (Regularization parameter) on this model to find which works best, and chose a value which gave least loss. After that I tried some decision tree models but they did not perform as well. Next, I tried to synthetically generate data with SMOTE (since my dataset was small). I know SMOTE is supposed to be used for fixing skewed distributions, my dataset was not very skewed, but I found no better alternative, so I went with it. I did not yield any better results, so I stuck with my old 4 layer NN with hyper-tuned lambda.

c) The code should run fine in any Jupyter Notebook. (Don't use Colab or Kaggle) Note - If some of the losses come out to be very high, just rerun the cell, you will get the correct loss roughly in the same range. Also don't forget to replace the path of the dataset with its respective path in your system.

d) Screenshots -

![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(301).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(302).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(303).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(304).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(305).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(306).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(307).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(308).png)
![alt text](https://github.com/aritrar23/PClub-Task2-ML/blob/main/ScreenShots/Screenshot%20(309).png)
