
<!-- Make this private until publishing -->

# bean_disease
## Deep learning models for image-based bean leaf disease classification

Automated bean leaf disease classification by prototype machine learning models to classify three leaf conditions: angular leaf spot, bean rust or healthy.<br/>

### ▫️  PROPOSED MODELS
Custom architecture: **Bean-CNN (baseline CNN)**, **Bean-CNN-LSTM (hybrid CNN-LSTM)** <br/>
Pretrained adaptations: **EfficientNet-B7 + FC**, **EfficientNet-B7 + LSTM** <br/>

### ▫️ DEVELOPMENT ENVIRONMENT
Custom models were developed in Python and TensorFlow 2.17.0. Our custom ML models are verified against Python 3.10.12 and 3.12.4, TensorFlow 2.16.0 and 2.17.0 on Jupyter Notebook (Windows 11, macOS Sequoia 15.0.1) and Google Colab (Linux Ubuntu 22.04 LTS). The further experiments with EfficientNet were carried out with PyTorch 2.6.0 on Kaggle's P100 GPU. <br/>

### ▫️ SUMMARY
Using the [ibean dataset](https://github.com/AI-Lab-Makerere/ibean/) by Makerere AI Research Lab, we developed our models by integrating CNN with LSTM.

#### 1. Initial experiments<br/>
Five additional training sets were created using various augmentation methods: increased brightness, cropping, flipping, rotation, and the multi-technique combination.<br/> For these experiments, each training dataset contains 2715 images. 
The custom models (Bean-CNN and Bean-CNN-LSTM) were developed on the original dataset, and then trained further on all augmented sets.<br/>
Each Jupyter Notebook contains one model development process and uses the identical code with different training sets. <br/> 
This repo contains 3 notebook files showing the custom model development: <br/>
original Bean-CNN (905 training samples), original Bean-CNN-LSTM (905 training samples) and the best custom model Bean-CNN-LSTM (on the flip set with 2715 samples). The details of data is decribed below.
<br/>
<br/>
▪️Data description
<table>
  <tr>
    <th>Set</th><th>Sample size</th>
  </tr>
  <tr>
    <td>Training-Original<br/>
    Training-Increased brightness<br/> 
    Training-Combination<br/> 
    Training-Cropping<br/> 
    Training-Flipping<br/> 
    Training-Rotation<br/> 
    </td>
    <td>905<br/> 
      2715<br/> 
      2715<br/> 
      2715<br/> 
      2715<br/> 
      2715<br/> 
    </td>
  </tr>
  <tr>
    <td> Validation</td> <td>195</td>
  </tr>
  <tr>
    <td> Test</td><td>195</td>
  </tr>
</table>


#### 2. Extended experiments <br/>
The pretrained models were modified through fine-tuning process, and titled as EfficientNet-B7+FC and EfficientNet-B7+LSTM.
For these experiments, we used one training set, which was expanded by applying multiple augmentation methods (rotation, flips, scaling, blurring and contrast/brightness adjustment).<br/>
<br/>
▪️Data description
<table>
  <tr>
    <th>Set</th><th>Sample size</th>
  </tr>
  <tr>
    <td> Training</td><td>41,300</td>
  </tr>
  <tr>
    <td> Validation</td> <td>5,320</td>
  </tr>
  <tr>
    <td> Test</td><td>128</td>
  </tr>
</table>

#### 
<br/>



<br/>

🔷 **Important Note:** Due to the data size allowance limit, our data is stored in the [Huggingface](https://huggingface.co/datasets/hjin-r/bean_disease) repository.

<!-- Any comment goes here -->
