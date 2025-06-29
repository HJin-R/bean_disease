
<!-- Make this private until publishing -->

# bean_disease
### Image-based deep learning bean leaf disease classifier

Automated image-based bean leaf disease classification by prototype AI models to classify three leaf conditions: angular leaf spot, bean rust or healthy.<br/>

#### ▫️  Models
Custom Architecture: Bean-CNN (baseline CNN), Bean-CNN-LSTM (hybrid CNN-LSTM)<br/>
Pretrained Adaptations: EfficientNet-B7 + FC, EfficientNet-B7 + LSTM<br/>

#### ▫️ Development Environment
Custom models were developed in Python and TensorFlow 2.17.0. All ML models are verified against Python 3.10.12 and 3.12.4, TensorFlow 2.16.0 and 2.17.0 on Jupyter Notebook (Windows 11, macOS Sequoia 15.0.1) and Google Colab (Linux Ubuntu 22.04 LTS).<br/>

#### ▫️ Summary
Using the [ibean dataset](https://github.com/AI-Lab-Makerere/ibean/) by Makerere AI Research Lab, five additional training sets were created by different augmentation methods: increased brightness, crop, flip, rotation, and multi-technique combination.<br/> 
The initial models were developed on the original dataset and then trained further on all training sets.


<br/>


<!-- Any comment goes here -->
