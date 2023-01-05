# ResNet50 knowledge distillation
In this project a ResNet18 model is trained on CIFAR10 dataset by distilling a pretrained ResNet50 model which was pretrained on ImageNet dataset, and fine-tuned on CIFAR10.

Then the results from model distillation were compared to 1- ResNet18 trained from scrach alone, 2- and the fine-tuned pretrained ResNet50 itself.

---

## Results
The final results of training the above-mentioned models is as follows:

|      | **validation loss**  | **validation accuracy** |
|             ----------- | -----------  | -----------  |
| **RN-50 Last layer Fine-Tuned**       | 0.469        | 0.856        |
| **RN-18 Distilled**      | 0.582        | 0.783        |
| **RN-18 From scratch**        | 0.694        | 0.766        |
| **RN-50 Fully Fine-Tuned**         | 0.492        | 0.839        |

However, these are the results for training for a limited number of epochs. They may vary if continue training.
