# Resultados Completos dos Experimentos — WEKA Clash Royale

Este documento reúne **todas as saídas completas geradas no Weka** para os experimentos de classificação realizados com a base `emocao_jogador_clashroyale_v2`.  
Foram testados os seguintes algoritmos:

- ZeroR  
- OneR  
- J48  
- Naive Bayes  
- IBk  


---

## 🧩 Algoritmo: ZeroR

```text
=== Run information ===

Scheme:       weka.classifiers.rules.ZeroR
Relation:     emocao_jogador_clashroyale_v2
Instances:    200
Attributes:   7
vitorias_consecutivas
cartas_nivel_medio
tempo_partida_min
torres_destruidas
torres_perdidas
trofeus_delta
emocao_jogador
Test mode:    10-fold cross-validation

=== Classifier model (full training set) ===

ZeroR predicts class value: motivado

Time taken to build model: 0 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances          60               30      %
Incorrectly Classified Instances       140               70      %
Kappa statistic                          0

Mean absolute error                      0.3732
Root mean squared error                  0.432
Relative absolute error                100      %
Root relative squared error            100      %
Total Number of Instances              200

=== Detailed Accuracy By Class ===

             TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
             0,000    0,000    ?          0,000    ?          ?        0,500     0,250     feliz
             1,000    1,000    0,300      1,000    0,462      ?        0,500     0,300     motivado
             0,000    0,000    ?          0,000    ?          ?        0,464     0,214     neutro
             0,000    0,000    ?          0,000    ?          ?        0,464     0,214     frustrado

Weighted Avg.    0,300    0,300    ?          0,300    ?          ?        0,484     0,249

=== Confusion Matrix ===

a  b  c  d   ⟵ classified as
0 50  0  0 |  a = feliz
0 60  0  0 |  b = motivado
0 45  0  0 |  c = neutro
0 45  0  0 |  d = frustrado
```
## 🧩 Algoritmo: OneR
```text
=== Run information ===

Scheme:       weka.classifiers.rules.OneR -B 6
Relation:     emocao_jogador_clashroyale_v2
Instances:    200
Attributes:   7
vitorias_consecutivas
cartas_nivel_medio
tempo_partida_min
torres_destruidas
torres_perdidas
trofeus_delta
emocao_jogador
Test mode:    10-fold cross-validation

=== Classifier model (full training set) ===

trofeus_delta:
< -9.5 → frustrado
≤ 11.0 → neutro
≤ 24.5 → motivado
> 24.5 → feliz
(200/200 instances correct)

Time taken to build model: 0 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances         199               99.5    %
Incorrectly Classified Instances         1                0.5    %
Kappa statistic                          0.9933
Mean absolute error                      0.0025
Root mean squared error                  0.05
Relative absolute error                  0.6698 %
Root relative squared error             11.5737 %
Total Number of Instances              200

=== Detailed Accuracy By Class ===

             TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
             1,000    0,000    1,000      1,000    1,000      1,000    1,000     1,000     feliz
             1,000    0,000    1,000      1,000    1,000      1,000    1,000     1,000     motivado
             1,000    0,006    0,978      1,000    0,989      0,986    0,997     0,978     neutro
             0,978    0,000    1,000      0,978    0,989      0,986    0,989     0,983     frustrado

Weighted Avg.    0,995    0,001    0,995      0,995    0,995      0,994    0,997     0,991

=== Confusion Matrix ===

a  b  c  d   ⟵ classified as
50  0  0  0 |  a = feliz
0 60  0  0 |  b = motivado
0  0 45  0 |  c = neutro
0  0  1 44 |  d = frustrado
```
## 🧩 Algoritmo: J48
```text
=== Run information ===

Scheme:       weka.classifiers.trees.J48 -C 0.25 -M 2
Relation:     emocao_jogador_clashroyale_v2
Instances:    200
Attributes:   7
vitorias_consecutivas
cartas_nivel_medio
tempo_partida_min
torres_destruidas
torres_perdidas
trofeus_delta
emocao_jogador
Test mode:    10-fold cross-validation

=== Classifier model (full training set) ===

J48 pruned tree
trofeus_delta <= -10: frustrado (45.0)
trofeus_delta > -10
|   trofeus_delta <= 10: neutro (45.0)
|   trofeus_delta > 10
|   |   trofeus_delta <= 24: motivado (60.0)
|   |   trofeus_delta > 24: feliz (50.0)

Number of Leaves  : 4
Size of the tree  : 7

Time taken to build model: 0 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances         199               99.5    %
Incorrectly Classified Instances         1                0.5    %
Kappa statistic                          0.9933
Mean absolute error                      0.0025
Root mean squared error                  0.05
Relative absolute error                  0.6698 %
Root relative squared error             11.5737 %
Total Number of Instances              200

=== Detailed Accuracy By Class ===

             TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
             1,000    0,000    1,000      1,000    1,000      1,000    1,000     1,000     feliz
             1,000    0,000    1,000      1,000    1,000      1,000    1,000     1,000     motivado
             1,000    0,006    0,978      1,000    0,989      0,986    0,997     0,978     neutro
             0,978    0,000    1,000      0,978    0,989      0,986    0,989     0,983     frustrado

Weighted Avg.    0,995    0,001    0,995      0,995    0,995      0,994    0,997     0,991

=== Confusion Matrix ===

a  b  c  d   ⟵ classified as
50  0  0  0 |  a = feliz
0 60  0  0 |  b = motivado
0  0 45  0 |  c = neutro
0  0  1 44 |  d = frustrado
```
## 🧩 Algoritmo: Naive Bayes
```text
=== Run information ===

Scheme:       weka.classifiers.bayes.NaiveBayes
Relation:     emocao_jogador_clashroyale_v2
Instances:    200
Attributes:   7
vitorias_consecutivas
cartas_nivel_medio
tempo_partida_min
torres_destruidas
torres_perdidas
trofeus_delta
emocao_jogador
Test mode:    10-fold cross-validation

=== Classifier model (full training set) ===

Naive Bayes Classifier

                        Class
Attribute                 feliz      motivado     neutro     frustrado
(0.25)                    (0.3)       (0.23)       (0.23)
vitorias_consecutivas     mean 3.46   2.65         1.3778     0.8667
                          std. dev. 1.0042 1.0928  1.1213     0.8589
cartas_nivel_medio        mean 13.46 12.4167 11.3778 10.2667
tempo_partida_min         mean 2.9916 3.4709 4.0038 3.6853
torres_destruidas         mean 3.12 2.4167 1.5556 0.6222
torres_perdidas           mean 0.54 1.4167 1.4 2.8889
trofeus_delta             mean 31.0824 17.9793 1.1805 -20.8851

Time taken to build model: 0 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances         198               99      %
Incorrectly Classified Instances         2                1      %
Kappa statistic                          0.9866
Mean absolute error                      0.0193
Root mean squared error                  0.0767
Relative absolute error                  5.1617 %
Root relative squared error             17.7577 %
Total Number of Instances              200

=== Detailed Accuracy By Class ===

             TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
             0,980    0,000    1,000      0,980    0,990      0,987    1,000     1,000     feliz
             1,000    0,007    0,984      1,000    0,992      0,988    1,000     1,000     motivado
             0,978    0,000    1,000      0,978    0,989      0,986    1,000     0,999     neutro
             1,000    0,006    0,978      1,000    0,989      0,986    1,000     1,000     frustrado

Weighted Avg.    0,990    0,004    0,990      0,990    0,990      0,987    1,000     1,000

=== Confusion Matrix ===

a  b  c  d   ⟵ classified as
49  1  0  0 |  a = feliz
0 60  0  0 |  b = motivado
0  0 44  1 |  c = neutro
0  0  0 45 |  d = frustrado
```
## 🧩 Algoritmo: IBk
```text
=== Run information ===

Scheme:       weka.classifiers.lazy.IBk -K 1 -W 0 -A 
"weka.core.neighboursearch.LinearNNSearch -A 
\"weka.core.EuclideanDistance -R first-last\""
Relation:     emocao_jogador_clashroyale_v2
Instances:    200
Attributes:   7
vitorias_consecutivas
cartas_nivel_medio
tempo_partida_min
torres_destruidas
torres_perdidas
trofeus_delta
emocao_jogador
Test mode:    10-fold cross-validation

=== Classifier model (full training set) ===

IB1 instance-based classifier
using 1 nearest neighbour(s) for classification

Time taken to build model: 0 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances         184               92      %
Incorrectly Classified Instances        16                8      %
Kappa statistic                          0.8928
Mean absolute error                      0.0473
Root mean squared error                  0.1981
Relative absolute error                 12.6702 %
Root relative squared error             45.8563 %
Total Number of Instances              200

=== Detailed Accuracy By Class ===

             TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
             0,980    0,000    1,000      0,980    0,990      0,987    0,990     0,985     feliz
             0,933    0,029    0,933      0,933    0,933      0,905    0,953     0,891     motivado
             0,778    0,032    0,875      0,778    0,824      0,778    0,862     0,730     neutro
             0,978    0,045    0,863      0,978    0,917      0,894    0,963     0,849     frustrado

Weighted Avg.    0,920    0,026    0,921      0,920    0,919      0,894    0,944     0,869

=== Confusion Matrix ===

a  b  c  d   ⟵ classified as
49  1  0  0 |  a = feliz
0 56  4  0 |  b = motivado
0  3 35  7 |  c = neutro
0  0  1 44 |  d = frustrado
```
