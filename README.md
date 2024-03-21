# Descriptions

- This model is a segmentation model designed to segment the bile duct in Pure Laparoscopic Donor Hepatectomy (PLDH) for Living Donor Liver Transplantation (LDLT). It can help with the anatomical understanding of the biliary structure.
- The model is constructed using the DeepLabV3+ architecture with ResNet50 as an encoder. It was trained with 5-fold cross-validation on 300 images extracted from surgery videos of 30 patients who underwent PLDH surgery.

## Usage

- You can reproduce this model using jupyter notebook we provided
- You just need to modify the `model_path` and `video_path` within the ‘inferece.ipynb’ file.
- you can also download the model weights and a sample video from the link below.
    - https://1drv.ms/f/c/9db2e01a687d3baf/Eg-0KAOhkxxPl5UBGBRjX7ABuhzL9Zm6A7uwc5zZfEgPdg?e=0vYW67

## Preview

**Original video**

![output_fps1_1.gif](https://prod-files-secure.s3.us-west-2.amazonaws.com/1d3c01f1-fefd-4405-a57b-d5baf628540e/7967c888-ceba-428b-a503-b9277ec11bc8/output_fps1_1.gif)

**Inferenced video**

![inferenced_test_video.gif](https://prod-files-secure.s3.us-west-2.amazonaws.com/1d3c01f1-fefd-4405-a57b-d5baf628540e/120763bf-f9c2-42d3-92ab-c36e5b12eaa4/inferenced_test_video.gif)

## Requiremenets

pytorch==2.2.1

opencv==4.6.0

albumentations==1.3.1

segmentation-models-pytorch==0.3.1

numpy==1.26.4