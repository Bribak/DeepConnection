# DeepConnection
Deep learning model to classify relationship state in romantic couples from images and video.

This repository contains the code for training and using the deep learning binary classification model DeepConnection (described in 'DeepConnection: Classifying Relationship State from Images of Romantic Couples' by Maximiliane Uhlich and Daniel Bojar, https://psyarxiv.com/df25j/). Capitalizing on image data of romantic couples, DeepConnection uses facial and bodily expressions to predict the relationship state of the couple. This leads to a classification accuracy of nearly 97%.

DeepConnection consists of a pretrained ResNet-34 base model, with a subsequent spatial pyramid pooling layer (https://arxiv.org/abs/1406.4729, with spatial bins of [8x8], [4x4], [2x2], and [1x1]) and a power mean transformation (http://lamda.nju.edu.cn/zhangcl/papers/pm2018_pr.pdf). Subsequent to this, a fully connected part with dropout and ReLU activation layers leads to the binary prediction. The motivation for DeepConnection stems from an improved classification accuracy, a substantial increase in classification speed in comparison to manual coding schemes, and potentially new insights into relevant factors for relationship state in romantic couples.

The repository contains a Jupyter notebook with the relevant code for training & using the models. Additionally, representative trained models from the three stages discussed in the paper can be downloaded here (https://ln.sync.com/dl/04bec39c0/n8bei4rk-7kqhfkdz-u8vkgfkn-4kghsrpx) as pickle files.
