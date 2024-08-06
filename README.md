# Skin Disease Classification and Prediction

This project classifies skin diseases using deep learning models trained on the Kaggle skin disease dataset.

## Dataset

The dataset consists of images classified into the following categories:
1. Actinic keratosis
2. Atopic Dermatitis
3. Benign keratosis
4. Dermatofibroma
5. Melanocytic nevus
6. Melanoma
7. Squamous cell carcinoma
8. Tinea Ringworm Candidiasis
9. Vascular lesion

## **Link to Dataset**: https://drive.google.com/file/d/1lTzePvHIiaj8MwUiJNWErs9CZNaZKfsh/view?usp=sharing 

## Models Used

We experimented with several deep learning models for the classification task:

1. **InceptionV3**
2. **DenseNet**
3. **AlexNet**
4. **MobileNet** (showed the best results)

### Results

- **CNN**: Achieved 44% accuracy
- **InceptionV3**: Achieved 73% accuracy
- **MobileNet**: Achieved 85% accuracy

### Reason MobileNet Gave Better Results

MobileNet performed better due to its efficient architecture designed for mobile and embedded vision applications. It uses depthwise separable convolutions, which significantly reduce the number of parameters compared to standard convolutions, making the model lightweight yet powerful. This efficiency helps MobileNet generalize better, especially with smaller datasets. Yet, the overall accuracy is just 85% as the dataset was very small. 

## Conclusion

MobileNet outperformed other models in terms of accuracy for the skin disease classification task. Its architecture, which balances performance and computational efficiency, makes it particularly suitable for applications where resources are limited. 

## Future Work

1. **Increase Dataset Size**: Collect more images to improve model performance and generalization.
2. **Fine-tuning**: Experiment with fine-tuning other layers of MobileNet or different pre-trained models.
3. **Hyperparameter Tuning**: Perform extensive hyperparameter tuning to further improve accuracy.
4. **Ensemble Methods**: Combine predictions from multiple models to boost performance.
5. **Deploy Model**: Implement the model in a mobile or web application for real-time skin disease classification.
