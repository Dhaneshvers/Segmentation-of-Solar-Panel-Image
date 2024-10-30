# Sematic-Segmentation-of-Solar-Panel-Image
This project aims to accurately detect and segment defects in solar panels through deep learning techniques, utilizing the U-Net architecture with various high-performance backbones like ResNet34, VGG16, and InceptionV3. The primary objective is to enhance defect detection for practical applications in solar energy management.

![Solar Panel](https://images.takeshape.io/1f1d0876-be74-4b33-99c8-6ac93f1d70db/dev/34b0ddf2-dbd9-4945-bec0-858eacbf3410/hero-solar-close-up-cc-jake-haskell-2015.jpg?auto=compress%2Cformat&w=1200)


## Overview

The **Solar Panel Defect Segmentation** project focuses on leveraging deep learning techniques to detect and segment defects in solar panels accurately. Utilizing the U-Net architecture, this project implements various high-performance encoder backbones to enhance defect detection capabilities, making it suitable for real-world applications in renewable energy management.

## Key Features

The project encompasses several innovative features:

- **Image Preprocessing**: Images are resized to 256x256 pixels and normalized to maintain consistency during model training, ensuring that the network can learn effectively from the data.

- **Custom Loss Function**: A Jaccard loss function is employed, which is optimized for segmentation tasks to improve accuracy in detecting defects.

- **Model Training**: The implementation of the U-Net architecture with different encoder backbones (ResNet34, VGG16, InceptionV3) allows for capturing various defects, improving model robustness.

- **Evaluation Metrics**: The project evaluates performance using accuracy, Intersection over Union (IoU), and detailed classification reports, enabling a comprehensive assessment of model effectiveness.

- **Visualization**: The tool displays visual comparisons between original images, ground truth masks, and predicted masks, facilitating validation and interpretation of the segmentation results.

## High-Performance Models

### U-Net Architecture

The U-Net model is specifically designed for image segmentation, featuring a dual-path structure:

- **Contracting Path**: This part of the network captures contextual information through down-sampling, progressively extracting features from the input images.

- **Expanding Path**: This path restores the feature maps to their original dimensions, allowing for precise localization of defects. The use of skip connections between contracting and expanding paths helps retain essential spatial details.

### Encoder Backbones

1. **ResNet34**: A 34-layer residual network that effectively learns features in deeper networks using skip connections, providing a good balance of accuracy and efficiency.

2. **VGG16**: A straightforward 16-layer CNN that utilizes small 3x3 convolutional filters, excelling in capturing fine-grained details but requiring higher computational resources.

3. **InceptionV3**: This model employs Inception modules to capture multi-scale features, making it suitable for complex images with varying defect sizes, although it is more resource-intensive.

4.)  **efficientnetb4** : EfficientNetB4 is a convolutional neural network model that scales image resolution, depth, and width uniformly, offering high accuracy for detailed images with optimized resource efficiency.

## Dataset Requirements

The dataset for this project can be downloaded from [Zenodo](https://zenodo.org/records/10939100).Each image and mask should be resized to 256x256 pixels.

## Results

1. **ResNet34** :
                    **Loss vs val_loss**
   
![loss VS val_loss300](https://github.com/user-attachments/assets/83714788-77fb-4064-a645-de972ea8e063)


                   **Model Predicted Images**

![Output_image300](https://github.com/user-attachments/assets/80ab0be1-af9b-4c68-ad2f-9eb83b303596)



![val_accuracy VS val_loss300](https://github.com/user-attachments/assets/4e96670d-75c8-4a96-b0c6-82e8906b2bfd)


2. **VGG16**:
   
![loss VS val_loss300](https://github.com/user-attachments/assets/193fc475-7e4a-4a98-bd72-c737e4b5ca87)


![Output_image300](https://github.com/user-attachments/assets/b3df6610-7b06-4ce7-90da-0197f158c4a5)


![val_accuracy VS val_loss300](https://github.com/user-attachments/assets/88a87ff8-ec47-4348-9b10-6ad4f0e4757b)


3.) **InceptionV3**

![loss VS val_loss300](https://github.com/user-attachments/assets/15011017-c2ae-4926-af1f-2af2b942d7e1)


![Output_image300](https://github.com/user-attachments/assets/00a89e98-763e-4aa7-8dba-1f8193379008)


![val_accuracy VS val_loss300](https://github.com/user-attachments/assets/3d737497-d219-4441-9066-c1bb4878e7e4)


4.)  **efficientnetb4** :

![loss VS val_loss300](https://github.com/user-attachments/assets/965c7efd-3c5c-4932-8201-24c96c26ae4a)


![Output_image300](https://github.com/user-attachments/assets/05bebc92-1e3f-4a22-ae3e-6eef93ba260c)


![val_accuracy VS val_loss300](https://github.com/user-attachments/assets/4600e987-e82d-44d5-8105-3b64343989b6)


## Conclusion

This project represents a significant advancement in solar panel defect detection, contributing to the efficiency and reliability of solar energy systems. By employing sophisticated deep learning techniques, it enables stakeholders to better manage and maintain solar infrastructure, ultimately supporting the growth of renewable energy sources.
