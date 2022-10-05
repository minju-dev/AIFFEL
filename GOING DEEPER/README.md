# AIFFEL_Going-Deeper

### 1. ResNet Ablation Study
* 논문 [⌈**Deep Residual Learning for Image Recognition**⌋](https://arxiv.org/pdf/1512.03385.pdf)을 참조하여 ResNet 모델을 구현한다.
* Shortcut connection이 있는 모델과 없는 모델의 성능 차이를 확인한다. (**ResNet Ablation Study**)
#### [Model Implementation]
  1) ResNet-34
  2) ResNet-50
  3) Plain-34 : ResNet-34 모델에서 Shortcut connection만 빠진 모델
  4) Plain-50 : ResNet-50 모델에서 Shortcut connection만 빠진 모델

### 2. Image Augmentation
* Augmentation 적용에 따른 모델의 성능을 비교해본다. 
#### [Augmentation Model]
  1) No Augmentation
  2) 기본 Augmentation
  3) CutMix
  4) Mixup
  5) 기본 Augmentation + CutMix
  6) 기본 Augmentation + Mixup

### 3. Class Activation Map 
* CAM을 활용해서 물체의 위치를 찾는 object detection을 수행하고 이를 정답 데이터와 비교해본다.
### [Model]
  1) CAM
  2) Grad-CAM
  3) Detection with CAM, Grad-CAM (Bounding Box, IoU)
