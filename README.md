# ML_RandForests
As part of Machine Learning workshops organized by the student association 42AI, we prepared a two hours presentation about Decision Trees, Random Forets and Boosted Trees.

You can check out the slides here : https://docs.google.com/presentation/d/1FpmeAQrfIjwVHDyz84ZrBuyr3kaY2SbhG4EFn4YB8mg/edit?usp=sharing

Then we prepared a set of exercises so student can put the theory into practice ! Feel free to check it out :) 

## Work on the exercises (Jupyter needed)

```
git clone https://github.com/barthelemyleveque/ML_RandForests/
cd ML_RandForests
jupyter notebook decision_tree_exo.ipynb
```

The goal is to build a decision tree that will help us classify fruits depending on their characteristics :

Is color == Yellow?
--> True:
  Predict {'Lemon': 20}
--> False:
  Is season == Winter?
  --> True:
    Is color == Red?
    --> True:
      Predict {'Orange': 20}
    --> False:
      Predict {'Kiwi': 22}
  --> False:
    Is season == Summer?
    --> True:
      Predict {'Grape': 19}
    --> False:
      Predict {'Apple': 19}
