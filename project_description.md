# Project Description

#### Backgorund 
Sex differences in the language network is a long lasting and unresolved debate in the neuroscience field. Clinical studies have shown that pathologies or developmental conditions affecting language functions can differently affect individuals based on their sex (Cahill, 2006; Icer et al., 2020).

Although the language network is bilaterally organized, the left hemisphere is dominant for language in most individuals (Knect et al., 2000). Differences between men and women in the functional language network could explain sex differences in clinical conditions and offer insight for the development of interventions based on individuals’ characteristics. However, whether and how sex impacts the functional language network organization is still largely unknown
#### Objectives
In the present project, we address the research question on whether young adult individuals present differences in the pattern of rs-fMRI functional connectivity within the language network based on their sex. To address this issue, we propose to determine whether we can classify healthy young adult men and women, based on their rs-fMRI functional connectivity profiles within the language network. 
#### Data
The rs-fMRI images were issued from the human connectome project (HCP) S1200 release datatbase (Van Essen et al., 2012). The rs-fMRI images of a total of 667 healthy adults (322 men and 345 women, age: 22-35 years) were included in the study. First, for each participant, we extracted the functional connectivity networks anchored in the core regions of the language network from rs-fMRI data. This step is completed. 

With the knowledge acquired from this class, I will test whether machine learning models can accurately classify men and women based on their functional connectivity language maps within the language network. Subsequently, I will determine which are the most discriminant functional connectivity features that allow this classification.

### Plan: 
1. Make sure all participants have the same number of voxels 
   - For now : chose the intersection of all masks since each participant has a different brain mask applied :( 
   - After this class : redo seed-to-voxel correlation and apply the SAME brain mask for all participants 
2. Start with dimensionality reduction 
    - Principal Component Analysis
    - Find the number of features that explain maximum variance 
3. Classifier [ à déterminer]
    - Cross-validation 

### I expect to use the following tools, technologies, and libraries for this project:
- Git
- GitHub
- Visual Studio Code
- Jupyter Notebook
- Data Visualization (matplotlib, seaborn, plotly, pywidgets)
- Machine learning packages (nilearn, scikit-learn)
- Bash Terminal

### Deliverables 
-  Seed-to-voxel code 
-  Jupyter notebook containing Linear SVC model and accuracy 
-  Presentation slides
-  Project Report

## Results 
![image](https://user-images.githubusercontent.com/90349544/181355670-ace0976a-4cae-40c4-a38d-f82f1b58c3fe.png)

Results from the PCA determining the best number of features to include in our model. If this case, 0 features represent the best way to explain the max variance 

#### Results from the Linear SVC classifier 

/home/xlajoie/Pictures/Screenshot from 2022-07-27 15-31-33.png

accuracy (r2) = 0.875

Interpretation: the classifier was able to classify men and women with an accuracy of 87.5% 

