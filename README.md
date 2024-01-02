# Smart Contract Vulnerability Detection

# About this project

Smart contracts, the autonomous and self-executing pieces of code operating on blockchain platforms, have become integral to decentralized applications and blockchain ecosystems. However, their widespread adoption has given rise to the critical issue of vulnerabilities. This project addresses the challenge of smart contract vulnerability detection by harnessing the power of machine learning techniques. Traditional methods, such as manual code review and auditing, can be time-consuming and may overlook subtle issues. Using machine learning algorithms, this project efficiently analyzes smart contract code to identify potential vulnerabilities.

The following [dataset](https://github.com/mwritescode/slither-audited-smart-contracts) was used. The models were used: ResNet, DenseNet, AlexNet, and VGG. The results for the test set can be seen below. All the models were trained on 12 epochs except the last one.

The link for the weights can be found [here](https://drive.google.com/drive/folders/1r4Pc4udn9MCIdqCzI6S2GWLbtxyCVDVM?usp=drive_link).

|      Model Name     | Training time (mins) | Test accuracy (%) | F1 | Precision | Recall |
|:-------------------:|:--------------------:|:-----------------:|:--------:|:---------:|:------:|
|       Resnet18      |         55.8         |       58.79       |   72.14  |   77.41   |  68.14 |
|       Resnet34      |         65.0         |       57.34       |   70.34  |   78.69   |  64.18 |
|       Resnet50      |         90.4         |       54.40       |   68.29  |   76.60   |  62.20 |
|       Alexnet       |         44.6         |       52.86       |   66.83  |   75.65   |  60.49 |
|     Densenet121     |         98.4         |       48.22       |   63.06  |   72.40   |  56.90 |
|        VGG11        |         86.2         |       59.14       |   72.74  |   77.96   |  68.78 |
| Resnet18  38 epochs |         176.8        |       62.48       |   73.93  |   79.25   |  69.79 |

# Built With
* Python
* PyTorch