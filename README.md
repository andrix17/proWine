# proWine
Research on wine's properties base on grape variety and creation of classifiers using textual reviews.

## Directory structure

* dataset: it contains original dataset downloaded from https://www.kaggle.com/zynicide/wine-reviews;
* notebook: it contains notebook where I analyse the dataset:
  * ProWine.ipynb : analysis with LSA space with all reviews
  * ProWineWithSelection.ipynb : analysis with LSA space with wine reviews of limited number of grape variety
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
Riesling -> Precision:  0.776  Recall:  0.838  F1-Measure:  0.806
Cabernet Sauvignon ->
[1] "Precision:  0.787631271878646"
[1] "Recall:  0.683428957138036"
[1] "F1-Measure:  0.731839537405132"
[1] "Pinot Noir"
[1] "Precision:  0.858701298701299"
[1] "Recall:  0.811487481590574"
[1] "F1-Measure:  0.834427057041898"
[1] "Merlot"
[1] "Precision:  0.488593155893536"
[1] "Recall:  0.549732620320856"
[1] "F1-Measure:  0.517362858580775"
[1] "Chardonnay"
[1] "Precision:  0.847521865889213"
[1] "Recall:  0.825617722238001"
[1] "F1-Measure:  0.836426413465688"
[1] "Syrah"
[1] "Precision:  0.628066172276098"
[1] "Recall:  0.691582914572864"
[1] "F1-Measure:  0.658295964125561"
[1] "Sauvignon Blanc"
[1] "Precision:  0.689138576779026"
[1] "Recall:  0.724885095206829"
[1] "F1-Measure:  0.70656"
[1] "Nebbiolo"
[1] "Precision:  0.706781279847182"
[1] "Recall:  0.902439024390244"
[1] "F1-Measure:  0.79271558650241"

#### LSA Classifiers
