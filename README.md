
<!-- Make this private until publishing -->

# bean_disease
## Deep learning models for image-based bean leaf disease classification

Automated bean leaf disease classification by prototype machine learning models to classify three leaf conditions: angular leaf spot, bean rust or healthy.<br/>

### ▫️  PROPOSED MODELS
Custom architecture: Bean-CNN (baseline CNN), Bean-CNN-LSTM (hybrid CNN-LSTM) <br/>
Pretrained adaptations: EfficientNet-B7 + FC, EfficientNet-B7 + LSTM <br/>

### ▫️ DEVELOPMENT ENVIRONMENT
Custom models were developed in Python and TensorFlow 2.17.0. Custom ML models are verified against Python 3.10.12 and 3.12.4, TensorFlow 2.16.0 and 2.17.0 on Jupyter Notebook (Windows 11, macOS Sequoia 15.0.1) and Google Colab (Linux Ubuntu 22.04 LTS).<br/>

### ▫️ SUMMARY
Using the [ibean dataset](https://github.com/AI-Lab-Makerere/ibean/) by Makerere AI Research Lab, we developed our models by intergrating CNN with LSTM.

#### 1. Initial experiments<br/>
Five additional training sets were created using various augmentation methods: increased brightness, cropping, flipping, rotation, and the multi-technique combination.<br/> For these experiments, each training data contains 2715 images. 
The custom models (Bean-CNN and Bean-CNN-LSTM) were developed on the original dataset, and then trained further on all augmented sets.<br/>
<br/>
▪️Data description <br/>
<!--Training set: Original (905)<br/> Increased brightness (2715), Combination (2715), Cropping (2715), Flipping, Rotation (2715) <br/>
Validation set: 195 <br/>
Test set: 195 <br/>-->

<table>
  <tr>
    <th>Set</th><th>Sample size</th>
  </tr>
  <tr>
    <td> Training</td><td>Original (905)<br/> Increased brightness (2715)<br/> Combination (2715)<br/> Cropping (2715)<br/> Flipping (2715)<br/> Rotation (2715)</td>
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
For these experiments, we used one training set, which was expanded using the multiple augmentation method (rotation, flips, scaling, blurring and contrast/brightness adjustment).<br/>
<br/>
▪️Data description <br/>
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


<!-- Any comment goes here -->
