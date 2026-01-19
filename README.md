# Image_Identification_AI-or-Real_Computer-Vision

This project leverages deep learning to detect synthetic images from real art images using CNN, Resnet50, DenseNet121..

There are many benefits of AI image generation, but there are also several drawbacks, one of the most detrimental being misinformation. During the 2024 election cycle, the internet saw an influx of AI-generated images aimed at spreading “partisan narratives” (Jingnan, H., 2024), or acting as a form of political propaganda.

After Hurricane Helene in September of 2024, an image of a young girl crying while holding a puppy in a boat was spread around social media sites like X. The photo was shared by senators and national committee members, and the photo wasn’t flagged as being AI-generated until after it had already gone viral. This photo is a less drastic example of misinformation; however, AI generated images have become a large portion of “misinformation-associated images” (NBCUniversal News Group, 2024).

What?
Our aim in this project is to train and develop a convolutional neural network (CNN) model that is trained on a dataset of real versus AI-generated images that can instantly detect if images are AI-generated. We also wanted to compare our built-from-scratch CNN model with other pre-existing CNN models to compare the detection accuracy of each. 

Our comparative analysis of multiple CNN models for classifying AI-generated versus real images yielded several key insights relevant to both model development and practical deployment.

Firstly, CNN Model 2 demonstrated improved performance over CNN Model 1. 

This enhancement is primarily attributable to the implementation of more extensive data augmentation techniques (horizontal flips, rotations, zooms, width/height shifts) and robust regularization strategies.

The larger, denser fully connected layer (256 units), combined with early stopping and learning rate reduction callbacks, enabled CNN Model 2 to capture more complex visual features while effectively mitigating overfitting.

This observation aligns with established deep learning best practices, which emphasize the importance of data diversity and regularization for achieving robust performance in image classification tasks.

Secondly, the transfer learning models, specifically ResNet50 and DenseNet121, outperformed both custom-built CNN models in terms of classification accuracy and F1-score. These pretrained architectures, particularly DenseNet121, leveraged rich feature hierarchies learned from large-scale datasets like ImageNet.

This resulted in better generalization on our relatively small dataset1. This finding corroborates the well-documented effectiveness of transfer learning in scenarios where training data is limited, a common challenge in specialized applications such as misinformation detection.

Art Image: Real Or Ai-generated
