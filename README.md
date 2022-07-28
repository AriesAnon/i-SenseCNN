# i-SenseCNN

*This will contain the finished files regarding our design project from testing different datasets up to the final product. The code created in the Google Colab will also serve as a documentation for future references.*

*Description of finished files:*
*   `Meat_Quality_Assessment_TL_Test_Documentation.ipynb` -> Testing the transfer learning code from YouTube (see link in the code) using the meat quality assessment dataset. Conclusion: accuracy fluctuates really bad making it unusable. ***Epochs: 100***;
*   `Multiclass_Test.ipynb` -> Testing a code from YouTube and adjusting it to accomodate Inception_V3 and use transfer learning to train it with a custom dataset that has 6 classes. Conclusion: Training success as well as testing. Consider increasing number of samples per class as well as increasing the number of epochs to reach a goal of at least 90% accuracy upon evaluation. Training time increases significantly compared to previous testing. ***Epochs: 10***;
* `ConvertRawImagesUsingRawpy.ipynb` -> Converting RAW images to JPEG and save them to Google Drive. Additional codes are included for convenience like opening images and deleting folders.
* `FinalModel_v3.ipynb` -> Trained in a PC that has a 32 gb RAM since the splitting of dataset takes up too much of the RAM. Accuracy is very bad during deployment. Overfitting might be the problem. Not optimal.
* `PrefinalModel.ipynb` -> The dataset used is a compilation of images scraped from the web. Accuracy is better than FinalModel_v3. Still not optimal.
* `zoomed_out_images_raw.ipynb` -> The number of classes were simplified to three. The number of epochs reduced to 10. A prototype of the final model. Accuracy has increased significantly.
* `etma_dmeo.ipynb` -> Final model. Reduced the number of epochs to 3. A rule of thumb should be to stop the epochs to at around .90. Overfitting will happen if the model continues to train beyond this. Best accuracy achieved compared to the previous models. During deployment, it performs okay. There's still a problem where it sometimes does not identify a meat accurately when the background is not white. Suggestion: perform image segmentation first to the datasets so the background might be inconsequential.
