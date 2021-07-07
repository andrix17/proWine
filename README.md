# proWine
Research on wine's properties base on grape variety and creation of classifiers using textual reviews.

## Directory structure

* dataset: it contains original dataset downloaded from https://www.kaggle.com/zynicide/wine-reviews;
* notebook: it contains notebook where I analyse the dataset:
  * ProWine.ipynb : analysis of LSA space with all reviews
  * ProWineWithSelection.ipynb : analysis of LSA space with wine reviews of limited number of grape variety
  * Classifiers.ipynb : test various classifiers on dataset 

## Result

### Result of ProWine.ipynb
Frequenza Pinot Noir =  0.102  
R-Precision on Pinot Noir with query "sandalwood cola silky" = 0.391

Frequenza Chardonnay =  0.091  
R-Precision on Chardonnay with query "peaches sweetness caramel residual pears" = 0.364

Frequenza Cabernet Sauvignon =  0.073  
R-Precision on Cabernet Sauvignon with query "currant tannin mountain" = 0.346

Frequenza Riesling =  0.040  
R-Precision on Riesling with query "orange apricot juice freshness hints candied freshness" = 0.289

Frequenza Sauvignon Blanc =  0.038  
R-Precision on Sauvignon Blanc with query "green herbaceous mostly blanc chalky acid mix brings sense" = 0.309

Frequenza Syrah =  0.038  
R-Precision on Syrah with query "chocolate mocha power dark smoke tea tannin plums compact pomegranates" = 0.160

Frequenza Nebbiolo = 0,021  
R-Precision on Nebbiolo with query "dried crushed sage blue violet star anise clove chopped menthol whiff underbrush balsamic floor ground wild assertive finegrained provide emerge glass baking" = 0.349

### Result of ProWineWithSelection.ipynb
Frequenza Pinot Noir =  0.239  
R-Precision on Pinot Noir with query "oregon planted mushroom red gentle river" = 0.731

Frequenza Chardonnay =  0.211  
R-Precision on Chardonnay with query "tropical apricots apples crispness warm peaches" = 0.746

Frequenza Cabernet Sauvignon =  0.172  
R-Precision on Cabernet Sauvignon with query "blackberry cassis" = 0.615

Frequenza Riesling =  0.093  
R-Precision on Riesling with query "aromatic sweetness perfume intensity perfume" = 0.684

Frequenza Sauvignon Blanc =  0.088  
R-Precision on Sauvignon Blanc with query "green pure herbaceous ripeness blanc" = 0.465

Frequenza Syrah =  0.090  
R-Precision on Syrah with query "chewy smoke expression finishing depth fig layered" = 0.307

Frequenza Merlot =  0.056  
R-Precision on Merlot with query "cocoa flavorful" = 0.171

Frequenza Nebbiolo = 0.051  
R-Precision on Nebbiolo with query "underbrush mature grilled finegrained tightly" = 0.767

### Result of Classifiers.ipynb
#### TF-IDF Classifiers
##### Rocchio 
Accuracy: 0.765
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.859     | 0.811  | 0.834      |
| Chardonnay         | 0.847     | 0.826  | 0.836      |
| Cabernet Sauvignon | 0.788     | 0.683  | 0.732      |
| Riesling           | 0.776     | 0.838  | 0.806      |
| Sauvignon Blanc    | 0.689     | 0.725  | 0.707      |
| Syrah              | 0.628     | 0.691  | 0.658      |
| Merlot             | 0.489     | 0.550  | 0.517      |
| Nebbiolo           | 0.707     | 0.902  | 0.793      |

##### KNN 
Accuracy: 0.754
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.724     | 0.851  | 0.804      |
| Chardonnay         | 0.737     | 0.902  | 0.811      |
| Cabernet Sauvignon | 0.651     | 0.815  | 0.724      |
| Riesling           | 0.842     | 0.761  | 0.800      |
| Sauvignon Blanc    | 0.833     | 0.587  | 0.689      |
| Syrah              | 0.826     | 0.448  | 0.581      |
| Merlot             | 0.850     | 0.231  | 0.363      |
| Nebbiolo           | 0.898     | 0.900  | 0.899      |

##### Multinomial Naive Bayes 
Accuracy: 0.759
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.727     | 0.940  | 0.820      |
| Chardonnay         | 0.759     | 0.942  | 0.841      |
| Cabernet Sauvignon | 0.653     | 0.796  | 0.718      |
| Riesling           | 0.899     | 0.733  | 0.808      |
| Sauvignon Blanc    | 0.893     | 0.544  | 0.676      |
| Syrah              | 0.862     | 0.430  | 0.574      |
| Merlot             | 0.980     | 0.051  | 0.098      |
| Nebbiolo           | 0.987     | 0.843  | 0.909      |

##### Bernoulli Naive Bayes 
Accuracy: 0.759
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.652     | 0.899  | 0.756      |
| Chardonnay         | 0.675     | 0.954  | 0.791      |
| Cabernet Sauvignon | 0.747     | 0.672  | 0.708      |
| Riesling           | 0.960     | 0.549  | 0.699      |
| Sauvignon Blanc    | 0.762     | 0.637  | 0.694      |
| Syrah              | 0.862     | 0.340  | 0.489      |
| Merlot             | 0.529     | 0.400  | 0.455      |
| Nebbiolo           | 1.000     | 0.273  | 0.429      |

#### LSA Classifiers

##### Rocchio 
Accuracy: 0.612
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.836     | 0.634  | 0.721      |
| Chardonnay         | 0.809     | 0.692  | 0.746      |
| Cabernet Sauvignon | 0.687     | 0.506  | 0.583      |
| Riesling           | 0.682     | 0.785  | 0.730      |
| Sauvignon Blanc    | 0.511     | 0.689  | 0.587      |
| Syrah              | 0.314     | 0.419  | 0.359      |
| Merlot             | 0.174     | 0.319  | 0.225      |
| Nebbiolo           | 0.628     | 0.783  | 0.697      |

##### KNN 
Accuracy: 0.706
|                    | Precision | Recall | F1-Measure |
|--------------------|-----------|--------|------------|
| Pinot Noir         | 0.745     | 0.845  | 0.792      |
| Chardonnay         | 0.764     | 0.890  | 0.822      |
| Cabernet Sauvignon | 0.592     | 0.774  | 0.671      |
| Riesling           | 0.790     | 0.758  | 0.773      |
| Sauvignon Blanc    | 0.765     | 0.542  | 0.635      |
| Syrah              | 0.472     | 0.268  | 0.342      |
| Merlot             | 0.353     | 0.057  | 0.098      |
| Nebbiolo           | 0.842     | 0.778  | 0.809      |
