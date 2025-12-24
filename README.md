# Task 1: Food Classification (5 Types)

**Student:** Shamil Tahirov
**ID:** 8
**Seed:** 42

## Presentation
[View Presentation Slides](https://docs.google.com/presentation/d/1sFuJdAwlUyYn2yc6RnRm7iRK7pzwZdpL/edit?usp=drive_link&ouid=106015534459131964806&rtpof=true&sd=true)

## Dataset
- **Name:** Food-101 (subset: 5 food types)  
- **Classes:** 5  
- **Training samples:** 500 per class (total 2500)  
- **Test samples:** 100 per class (total 500)  

## Model Architecture
- **Type:** Simple CNN  
- **Convolutional layers:** 3  
- **Fully connected layers:** 2  
- **Total parameters:** ~100k  

## Training Comparison

### Version 1
- **Learning rate:** 0.001  
- **Batch size:** 16  
- **Optimizer:** Adam  
- **Test accuracy:** 80.0%

### Version 2
- **Learning rate:** 0.0005  
- **Batch size:** 32  
- **Optimizer:** Adam  
- **Test accuracy:** 85.0%

### Best Result
- **Best version:** Version 2  
- **Final test accuracy:** 85.0%  
- **Target accuracy:** 85.0%  
- **Status:** ✓ Achieved

## Analysis
- **Best performing class:** Pizza  
- **Worst performing class:** Sushi  
- **Key observations:**  
  - Increasing batch size and decreasing learning rate improved accuracy.  
  - Some classes are more visually similar, which increases misclassification.  
  - Model performs well on dominant features (like pizza toppings), struggles on subtle differences (like sushi types).

