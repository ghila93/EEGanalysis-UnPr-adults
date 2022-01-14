# Predictive motor activation: Modulated by expectancy or predictability?

## Abstract
Predicting actions is a fundamental ability that helps us to comprehend what is happening in our environment and to interact with others. The motor system was previously identified as source of action predictions. Yet, which aspect of the statistical likelihood of upcoming actions the motor system is sensitive to remains an open question. This EEG study investigated how regularities in observed actions are reflected in the motor system and utilized to predict upcoming actions. Prior to measuring EEG, participants watched videos of action sequences with different transitional probabilities at home. After training, participants’ brain activity over motor areas was measured using EEG while watching videos of action sequences with the same statistical structure. Focusing on the mu and beta frequency bands we tested whether activity of the motor system reflects the statistical likelihood of upcoming actions. We also explored two distinct aspects of the statistical structure that reflect different prediction processes, expectancy and predictability. Expectancy reflects participants’ expectation of the most likely action minimizing the cognitive load to the expense of the prediction’s flexibility. On the other hand, predictability, represents all possible actions and their relative probabilities maximizing the flexibility of the prediction at the expenses of a higher cognitive load. Results revealed that mu and beta play different roles during action prediction. While the mu rhythm reflected anticipatory activity without any link to the statistical structure, the beta rhythm was related to the expectancy of an action. Our findings support theories proposing that the motor system underlies action prediction, and they extend such theories by showing that multiple forms of statistical information are extracted when observing action sequences. This information is integrated in the prediction generated by the neural motor system of which action is going to happen next.


## Scripts

Code used to perform frequency analysis on adults EEG data.
The script are using [Fieltrip](http://www.fieldtriptoolbox.org/) toolbox to compute the analysis.

The analysis is divided in two parts:
- the first relative to the extraction of the sample specific mu and beta roladic rythms during an action execution task
- the second relative to the analysis during the observation adn rpediciton of actions

Files:
- Functions_##.m                  = contain fucntion that will be called by the Preprocessing_##.m scripts.
- Preprocessing_##.m              = basic prerocessing and ICA of the EEG data 
- Main_##.m                       = extract log-normalized index of freequency power
- Info_var.m                      = contain general information valid both for Functions/Preprocessing/Main
- trial_fun_##.m                  = allow specific epochs segmentation
