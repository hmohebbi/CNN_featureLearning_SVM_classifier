# Image Classification via Transfer Learning

In this project, a small subset of the <a href="http://www.image-net.org/">ImageNet</a> has been used as a dataset. Three classes of Piano, Saxophone, and Violin, the number of images per class is limited to 600 images.

In the feature learning phase, the images are fed to a pre-trained Densely Connected Convolutional Networks (<a href="http://openaccess.thecvf.com/content_cvpr_2017/papers/Huang_Densely_Connected_Convolutional_CVPR_2017_paper.pdf">DenseNet</a>)-proposed by G Huang and et al in CVPR 2017- that top layer was removed and all convolutional layers have been frozen. 

Finally, both Support Vector Machine (SVM) and Fully Connected (FC) classifiers have been used to classify the extracted features and the results have been reported.

For SVM, t-distributed stochastic neighbor embedding (t-SNE) and Principal Component Analysis (PCA) have been used to transform features into a 2-d and 3-d feature space. For FC, all convolutional DenseNet layers have been frozen and only top layers (FC) have been trained.

