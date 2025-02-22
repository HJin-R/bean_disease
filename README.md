# bean_disease
Bean leaf disease classification 

#### THIS REPOSITORY IS BEING UPDATED.

### Bean-CNN-LSTM and Bean-CNN

Automated image-based bean leaf disease classification prototype AI models to classify three leaf conditions: angular leaf spot, bean rust or healthy.<br/>
Prototype AI models were developed in Python and TensorFlow 2.17.0. All models included in the artefact directory are verified against Python 3.10.12 and 3.12.4, TensorFlow 2.16.0 and 2.17.0 on Jupyter Notebook (Windows 11, macOS Sequoia 15.0.1) and Google Colab (Linux Ubuntu 22.04 LTS).Bean-CNN (baseline CNN) and Bean-CNN-LSTM (hybrid CNN-LSTM).<br/>


Using the [ibean dataset](https://github.com/AI-Lab-Makerere/ibean/) by Makerere AI Research Lab, five additional training sets were created by different augmentation methods: increased brightness, crop, flip, rotation, and multi-technique combination.<br/> 
The initial models were developed on the original dataset and then trained further on all training sets to examine which architecture and training sets were more advantageous to performance.

<br/>
