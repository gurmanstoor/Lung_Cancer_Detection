# Lung Cancer Detection using Convolutional Neural Network

### Notes:
Data can be found at [this link](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images?resource=download&select=lung_colon_image_set)


To run this model, please place the provided lung_colon_image_set.zip file in the Content folder alongside, but not in, the sample_data folder.


In order to increase the efficiency of which this model runs, and to avoid the epochs taking multiple hours, please change this runtime to use TPU. This can be done by selecting the Runtime tab in the toolbar and selecting "Change Runtime Type" then select "TPU" from the dropdown. The other TPU optimization configurations have already been added to the code below.

<br>

### Discussion
The data that I used for this implementation is not the full data set. In order to save on uploading and processing time, I selected 1000 of the 5000 images in each of the case folders of Lung benign tissue, Lung adenocarcinoma, and Lung squamous cell carcinoma images. 

<br>

Although this saves time to upload the files, and would have most likely allowed me to finish the challenge within the original allotted time frame, It does affect the accuracy of the model. 

<br>

The accuracy of this model is unfortunately below a score that I would have liked. To try and improve this, I decreased each batch size to improve accuracy due to reduced generalization error and faster convergence. I also increased the training split to provide the model with more data. Taking a look at the data, it does appear there is some overfitting occuring which could explain the scores.

<br>

To improve the accuracy further, The best option would be to use more data, however in this context where we are constrained, I would recomend increasing the number of Epochs. This would improve prediction accuracy by allowing the model to refine its parameters and learn more complex patterns in the data. However I would advise that care must be taken to prevent overfitting and ensure the model generalizes well to new, unseen data.
