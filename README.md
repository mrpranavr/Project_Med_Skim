<head>
  <h1 align = "center"><b>Project Med Skim</b></h1><br>
</head>
<p align = "center">
  Using Natural Language Processing (Text classification) to skim through a large medical RCT abstract and returning a classified and ordered summary of the entire abstract for ease of reading. Next time anyone want to read through a long time consuming medical RCT abstract this will come in handy.
</p>

<p align ="center">
<img src="https://user-images.githubusercontent.com/88646272/139391309-fbcf3d35-ec6a-4bbd-bb87-c937b550ee8b.jpg" width = 30% height=30%>
</p>

## What does this project do ?
Lets say you have to read through a bunch of medical RCT paper abstracts to know the summary of the paper. Most of the papers have their abstract in the form of a long lengthy paragraph and reading through the entire paragraph just to find the method or background specifically, can be time consuming.

Thats where this model comes in. This model takes in the lengthy paragraph as the input and can return a well ordered and labelled summary of the abstract. So now you can just read what you want to read.

For example, look at the abstract below,

<b>"This RCT examined the efficacy of a manualized social intervention for children with HFASDs. Participants were randomly assigned to treatment or wait-list conditions. Treatment included instruction and therapeutic activities targeting social skills, face-emotion recognition, interest expansion, and interpretation of non-literal language. A response-cost program was applied to reduce problem behaviors and foster skills acquisition. Significant treatment effects were found for five of seven primary outcome measures (parent ratings and direct child measures). Secondary measures based on staff ratings (treatment group only) corroborated gains reported by parents. High levels of parent, child and staff satisfaction were reported, along with high levels of treatment fidelity. Standardized effect size estimates were primarily in the medium and large ranges and favored the treatment group."</b>

Readin through one of these may be fine, but imagine reading through tens of these just to write a summary about its background. Time consuming right?

Now look at the output the model gives once you pass this sentence through the model

![Capture2](https://user-images.githubusercontent.com/88646272/139393710-60e332ef-2631-4643-88d0-c4d890ef82cd.PNG)

Much better readable right ? Exactly ! Now if you just want the background or the conclusion, you can easily read it out instead of reading the entire abstract.

###  Model architecture

The architecture for the model is deeply inspired from the paper - <b>Neural Networks for Joint Sentence Classification
in Medical Paper Abstracts</b> found here: https://arxiv.org/pdf/1612.05251.pdf. 

The model architecture they used in their paper is : 

<p align="center">
<img src= "https://user-images.githubusercontent.com/88646272/139394318-44ac1a5a-1aec-4f35-9829-511a60150da1.png">
</p>

The model architecture used for this project is as below:

<p align = "center">
<img src= "https://user-images.githubusercontent.com/88646272/139394467-a196c7dc-f5ba-4589-a3d1-905cb9e69e90.png">
</p>

<b>The colab file will contain step by step instruction on how to do the project. Make sure to enable the `GPU` computing in colab for increasing training speed.</b> 
