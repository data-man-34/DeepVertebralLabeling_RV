# DeepVertebralLabeling_RV
![DeepVertebralLabeling_Net overview](/img/DeepVertebralLabeling_Net.png "DeepVertebralLabeling_Net overview")

### Overview
<p align="justify">
For the diagnosis and monitoring of various diseases in the spine and the central nervous system, the detection and labeling of vertebrae in magnetic resonance imaging (MRI) is useful. Although several automatic methods for the detection and labeling of vertebrae have been developed, this is still an open task in which many improvements can be made. One way to detect the vertebra is to focus on the intervertebral discs (IVD), which are natural spacers between vertebrae. In this work, we present a set of convolutional networks (CNN) that perform regression for the detection and labeling of the IVD. The entry for each of the CNNs is the midsagittal plane image of the acquired volume. Each CNN is in charge of detecting one intervertebral disc, so the labeling is done implicitly. The output of each CNN is the coordinate (x, y) of the located IVD. We have done the training with the first 6 IVD (C2-C3 to C7-T1) using a total of 631 images with a pixel resolution of 1mm x 1mm. The mean error is between 2.98.mm and 4.33mm, the standard deviation range is between ±2.45 and ±3.45. Such results are competitive with the state of the art but require significantly less computational resources (estimated 2x) than other architectures based on fully convolutional networks.
</p>

Error distribution:
<p align="center">
<img src="/img/Error_violinplots.png" width="600">
</p>

<p align="justify">
<br/>

For more info please visit: [DeepVertebralLabeling_RV](https://www.researchgate.net/publication/326840620_Vertebral_labeling_on_MRI_using_deep_learning_techniques)

In this repository you can find the code for the model in Keras/Tensorflow.

### Citing DeepVertebralLabeling_RV
When citing DeepVertebralLabeling_VR in academic papers and thesis, please use this BibTeX entry:<br/>
</p>

    @inproceedings{Romero2018,
    address = {Montreal, QC, Canada},
    author = {Romero, Francisco Perdigon and David, Jean-Pierre and Cohen-Adad, Julien},
    booktitle = {NeuroInformatics 2018},
    doi = {10.13140/RG.2.2.33723.92962},
    title = {{Vertebral labeling on MRI using deep learning techniques}},
    url = {https://www.researchgate.net/publication/326840620{\_}Vertebral{\_}labeling{\_}on{\_}MRI{\_}using{\_}deep{\_}learning{\_}techniques},
    year = {2018}
    }

### License
MIT License <br/>
Copyright (c) 2018 Francisco Perdigon Romero
<p align="justify">
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
<p align="justify">
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
<p align="justify">
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
</p>
