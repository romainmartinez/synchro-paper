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
([permalink](https://romainmartinez.github.io/synchro-paper/v/863bd87d1e87fdae6ab1ff2f9c94b528fc3d58ad/))
was automatically generated
from [romainmartinez/synchro-paper@863bd87](https://github.com/romainmartinez/synchro-paper/tree/863bd87d1e87fdae6ab1ff2f9c94b528fc3d58ad)
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

In artistic swimming, about 40% of solo and team routine duration is spent with the head out of the water and most of that time is associated with the use of eggbeater kicks [@cOCMIvZK].
The eggbeater kick involves a complex combination of hip, knee and foot motions [@aThnaBqz; @rscUQMDF] to keep the body high above the water surface while performing artistic arm movements.
This water-treading technique is therefore a representative and important skill in artistic swimming, but also in water polo and lifesaving [@aThnaBqz].
Eggbeater kicks can be performed with both legs simultaneously (termed as “body-boost” or “dynamic”); or alternatively and continuously (termed as “sustained”).
In the latter case, a cyclical action is performed by left and right lower limbs in a similar motion but opposite in phase.
During team events, eggbeater kick is also needed during acrobatic moves (i.e. platforms, lifts and throws that involve up to 9 swimmers who propel or maintain another swimmer out of the water) by lower swimmers to create vertical propulsive force.
Height relative to the water surface is one of the key factors of performance and is evaluated using the FINA guiding scale for height (0 to 10 points with 0.5 resolution based on body landmarks) for both sustained and dynamic height [@EMbE5U2g].

From studies on water polo, the pattern of muscle activation during sustained eggbeater kick is a complex movement with high (up to 80%) levels of activation especially for the vastus medialis and the bicep femoris [@aThnaBqz; @Gf774x32].
Overall activities higher than 20% were reported for bi-articular (hip and knee) muscles that contribute to hip flexion-extension and abduction-adduction [@Gf774x32].
To the best of your knowledge, no study reported hip joint monoarticular muscle activities while Sanders [@G9nw32JQ] and Oliveira et al. [@Gf774x32] conclude that hip muscle strength, in addition to fast knee flexion and extension and speed of the feet should be optimized.
Oliveira et al. [@13wN9HgnX] found that a large abduction and flexion of the hips, as well as a fast extension and flexion of the knees are essential kinematic factors for  high level of performance.
Moreover, Homma et al. [@rscUQMDF] reinforce that knees should be maintained higher than hip joints to ensure a horizontal trajectory of the feet to create a continuous lift force, rather than oscillating drag force using upside-down feet movements.
Zinner et al. [@uOs7XTRn] also showed that water polo players with higher isometric hip abductor muscle strength performed better in eggbeater kick.
Hip joint strength appears as essential to maintain knee height and enable horizontal trPajectories against water resistance using a combination of hip internal-external rotation and knee flexion-extension.

To understand the relationship between technique and performance, qualitative models of sustained and dynamic heights have been proposed by Sanders et al. [@aThnaBqz].
They also proposed regression models to predict the height based on foot speed, range of knee extension and initial angle of the upper body with respect to the horizontal.
Sanders’ predictive models of sustained and dynamic height explain 90% and 79% of the variance (n=12, r=0.85; n=16 r=0.55, respectively).
Oliveira [@13wN9HgnX] and Homma [@rscUQMDF] also reported modest to strong correlations between height and kinematics variables such as orientation and speed of the limbs.
Unfortunately, these predictive models are based on small samples of swimmers (4<n<16) and were not cross-validated.
Furthermore, they cannot easily be used for personalizing swimmer’s conditioning since they rely on biomechanical parameters that require 3D kinematic analyses.
Since the ability to generate high foot velocities is related to muscular function [@Gf774x32], we hypothesize that hip joint strength could be used to predict eggbeater kick performance.
It is anticipated that eggbeater kick for sustained or dynamic height and vertical propulsive force requires different physical capacities and therefore need specific conditioning content.

A recent survey pointed out the superiority of advanced machine learning algorithms over multiple linear regressions (as used in Sanders [@aThnaBqz]) to predict physical capability (e.g. maximal oxygen uptake), because they account for complex nonlinear relationships between variables [@8QQByeMx].
Machine learning is gaining popularity in sports (e.g. in triathlon [@iUmDuGC6]; biathlon [@Dulx77Pa]; or track and field [@M4dO37MO]) as in most domains to predict performance.
A review of computational intelligence applications in sports underlined the need to develop artificial support systems that would help to design training plans, to measure indicators of an athlete’s readiness and to analyze data during training sessions [@MBEmmpnE].
To implement such systems, accurate performance prediction is crucial.
Gradient boosting algorithms are one possible approach to achieve such accuracy.
These are highly customizable and powerful tools for learning and analyzing problems with heterogeneous parameters and noisy data with complex interactions [@doYf0PkM].
The current study aims to investigate the relationship between hip function in elite artistic swimmers and performance in eggbeater kicks using gradient boosting algorithms.
The predictive model will be considered valid if its accuracy is similar to the FINA guiding scale for height resolution (0.5).
A secondary objective is to illustrate how the model can be used to develop an artificial conditioning support system.

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
