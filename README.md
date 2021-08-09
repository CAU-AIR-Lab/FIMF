# Fast Multi-label Feature Selection based on Information-theoretic Feature Ranking

## Abstract

Multi-label feature selection involves selecting important features from multi-label data sets. This can be achieved by ranking features based on their importance and then selecting the top-ranked features. Many multi-label feature selection methods for finding a feature subset that can improve multi-label learning accuracy have been proposed. In contrast, computationally efficient multi-label feature selection methods have not been studied extensively. In this study, we propose a fast multi-label feature selection method based on information-theoretic feature ranking. Experimental results demonstrate that the proposed method generates a feature subset significantly faster than several other multi-label feature selection methods for large multi-label data sets.

This program is designed to perform the feature selection for multi-label data set. This method deals with standard multi-label data set, in which the number of given label is larger than one.

This software is a Matlab implementation of proposed method, highy specialized on problems of categorical data set classification. The original version of this program was written by Jaesung Lee.

### [Paper]
Jaesung Lee and Dae-Won Kim, ["Fast Multi-label Feature Selection based on Information-theoretic Feature Ranking,"](https://www.sciencedirect.com/science/article/pii/S0031320315001338)
Pattern Recognition, 2015

## License

This program is available for download for non-commercial use, licensed under the GNU General Public License, which is allows its use for research purposes or other free software projects but does not allow its incorporation into any type of commerical software.

## Sample Input and Output

It will return the index of input binary features in orders of conditional dependency, named for user-specified variable. This code can executed under Matlab command window.

### [Usage]:
   `>> idx = fimf( features, labels, f_nums, l_nums );`

### [Description]
   features – a matrix that is composed of features \
   labels – a matrix represents labels of each pattern is assigned to \
   f_nums – the number of features to be actually examined for calculating their importance \
   l_nums – the number of labels to be actually examined for calculating label dependency

By convention in the input features matrix, rows represent data (e.g. patterns) and columns represent features.

The information for other programs are:

   `>> ent = b_entropy( features )` : Calculate the entropy of given (multivariate) binary feature
