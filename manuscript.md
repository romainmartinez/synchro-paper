---
author-meta:
- Romain Martinez
- "\xC9lodie Monga-Dubreuil"
- Najoua Assila
- Gauthier Desmyttere
- Mickael Begon
date-meta: '2019-07-05'
keywords:
- artistic swimming
- eggbeater kick
- machine learning
- hip joint function
lang: en-US
title: Predicting eggbeater kick performances from hip joint function testing in artistic
  swimming
...






<small><em>
This manuscript
([permalink](https://romainmartinez.github.io/synchro-paper/v/5f06f86db34826c94c161a88d4816633b388160e/))
was automatically generated
from [romainmartinez/synchro-paper@5f06f86](https://github.com/romainmartinez/synchro-paper/tree/5f06f86db34826c94c161a88d4816633b388160e)
on July 5, 2019.
</em></small>

## Authors



Romain Martinez^1[*](#correspondence)^,
Élodie Monga-Dubreuil^1^,
Najoua Assila^1^,
Gauthier Desmyttere^1^,
Mickael Begon^1^


1. School of Kinesiology and Exercise Science, Faculty of Medicine, University of Montreal

::: {#correspondence}
\* — correspondence preferred via [GitHub Issues](https://github.com/romainmartinez/synchro-paper/issues).
Otherwise, address correspondence to <martinez.staps@gmail.com>.
:::


## Abstract {.page_break_before}

Eggbeater kick is an important skill in artistic swimming to lift the body above water level.
Previous attempts to model eggbeater kick performance include complex biomechanical parameters that cannot be easily used to guide strength and conditioning training.
In this study, we modelled the relationship between hip function and eggbeater kick performance in 92 elite artistic swimmers with a machine learning algorithm.
We assessed hip function with six isometric tests that can be easily performed on a weekly basis, without the need for a physiotherapist or a scientist.
Our model may accurately predict future performances as the predictive error is similar to the resolution of the scale used by judges during competitions.
We then provide a set of interpretation and simulations methods that showcase some of the important predictors of the eggbeater kick performance and highlight personalized strategy to reach a target performance.
By using a model that is both accurate and interpretable, practitioners could access objective decision-making support, allowing them to effectively select athletes and design personalized conditioning programs.
We believe machine learning and data-driven decision-making provide sports scientists and coaches with new opportunities to enhance research and performance.


## Introduction

In artistic swimming about 40% of solo and team routine duration is spent with the head out of the water and most of that time is associated with the use of eggbeater kicks [@cOCMIvZK].
The eggbeater kick involves a complex combination of hip, knee and foot motions [@aThnaBqz; @rscUQMDF] to keep the body high above the water surface while performing artistic arm movements.
This water-treading technique is therefore a representative and important skill in artistic swimming, but also in water polo and lifesaving [3].
Eggbeater kicks can be performed with both legs simultaneously (termed as “body-boost” or “dynamic”); or alternatively and continuously (termed as “sustained”).
In the latter case, a cyclical action is performed by left and right lower limbs in a similar motion but opposite in phase.
During team events, eggbeater kick is also needed during acrobatic moves (i.e. platforms, lifts and throws that involve up to 9 swimmers who propel or maintain another swimmer out of the water) by lower swimmers to create vertical propulsive force.
Height relative to the water surface is one of the key factors of performance and is evaluated using the FINA guiding scale for height (0 to 10 points with 0.5 resolution based on body landmarks) for both sustained and dynamic height [5].

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
