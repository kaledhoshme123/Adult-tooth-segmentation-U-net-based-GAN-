# Adult tooth segmentation U-net based GAN 
- Dental segmentation for adults. Many dentists suffer from the difficulty of analyzing panoramic images of teeth for adults. One of the difficulties that dentists suffer from is the difficulty in determining the extension and root of the teeth, which affects the decisions of doctors in many cases that include dental implants, tooth extraction, or other problems. Cases experienced by dentists are difficult.
- In this study, it is proposed to use generative neuronal models in order to study more deeply the fragmentation process of teeth.
The use of generative networks helps to understand more deeply the shape in which the teeth can be formed, which helps in generalizing on the ability to segment the process, and this leads to models that are more understanding of the morphological structure of the teeth.
- A generative neural network was proposed with the aim of segmenting the dental region of adults, and after completing the process of training the generative network, the generator was retrained only according to the concept of pixel2pixel and freezing the weights of a number of layers, in order to make the generator network depend on the training it received from the generative neural network.
- The generative neural network achieved high results in the process of segmentation and tooth recognition, and those results were improved by retraining the generator with freezing a number of layers in order to make the generator able to generalize the results that were reached.
- I was able to reach a stable training process free from overfitting and other problems that could face the training process.
The number of samples included in the dataset is small, so generative neural networks were used to build a segmentation model that is more generalizable. Within the same panoramic medical images.
- In the beginning, the generative neural network will find it difficult to understand exactly what is required of it, but with time, the generative network will realize that it has to generate a mask so that if it is applied to the panoramic image, we will extract areas of the teeth with the same characteristics and specifications that the distinguished one studied.
- The main idea is to make the hashing task not easy and requires awareness on the part of the generator of what it should generate, since I did not tell it exactly what it should generate, but rather I left it to him to realize what he should generate.
As I mentioned, with time the generator will understand the idea and therefore will work on generating the mask without being asked to do so openly.
# Dataset used:
https://www.kaggle.com/datasets/truthisneverlinear/childrens-dental-panoramic-radiographs-dataset

# Samples of Dataset:
|  |
| :---:   |
| ![__results___10_1](https://github.com/kaledhoshme123/Adult-tooth-segmentation-U-net-based-GAN-/assets/108609519/3ec7e4ba-2ca9-4fe0-a655-678be0c1eeaf)|

# Results:
| Results | #validation data    | #training data    |
| :---:   | :---: | :---: |
| loss, accuracy, precision, recall |  ![image](https://github.com/kaledhoshme123/Adult-tooth-segmentation-U-net-based-GAN-/assets/108609519/195e76a7-1204-4253-85c6-7f271431fafe)|  ![image](https://github.com/kaledhoshme123/Adult-tooth-segmentation-U-net-based-GAN-/assets/108609519/bbec68b3-a79e-467c-9f3d-ecea31fc32ff)|

## Validation Data
![__results___51_0](https://github.com/kaledhoshme123/Adult-tooth-segmentation-U-net-based-GAN-/assets/108609519/a996f39d-ba2f-4760-83de-93792c11cd6b)

## Training Data
![__results___55_0](https://github.com/kaledhoshme123/Adult-tooth-segmentation-U-net-based-GAN-/assets/108609519/1ade9f3e-da88-4339-954e-e0f1ed686041)
