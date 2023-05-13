# Mutual-Information
The tool computes the mutual Information (MI) between several input variables xi (features) and an output y time series (target). 
For linear relations (e.g. by a linear mixing matrix) the mutual information serves as a mean to unmix the independent sources, see blind source seperation ICA.

Here, we have another question: Before analyzing the relations, what are the most important, essential features for predicting the output? For linear and non-linear functions y (x1,x2,..) the mutual information MI (y,x1,x2,..) is maximal for the essential inputs. In order to find them, the mutual information of order two (MI2) is computed between the target y(t) and

    each variable with different time delays or
    each input x in precondition on already selected,  better features with

          MI2( y(x) | x1*, x2*..) = max

 Thus, the input features are ranked due to their importance.
