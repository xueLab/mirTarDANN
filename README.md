# mirTarDANN
I) General Description:
- This package contains the python source code and optimized parameters of mirTarDANN, a meta-predictor for miRNA:mRNA interaction.
- All source codes are located under ./script
- All models are saved under ./model
- The user-generated input file should be saved under ./input
- The output of the meta-predictor will be found in ./result.


II) Additional packages required:
- Keras is required. Please find the installation information at https://keras.io/#installation. 
- TensorFlow is required as the backend engines for Keras. Please check https://www.tensorflow.org/install/. 


III) Usage:
1. python miRNA_mRNA_predictor.py
2. After seeing "Enter a path:", type in \miRNA_mRNA_predictor\
3. Then type in name of input file, which should end with "*.txt". For example, new.txt
4. The prediction is saved in ./result/new_result.txt
The input file should have six columns, including gene name, microRNA name, miRANDA mirSVR score, miRDB score, PITA score, and TargetScan context++ scores in each of the columns. If the score from an individual predictors is not available, please use "NA" in that column. Multiple inputs in the same file is also supported. In this case, please put one input in one line.
The result file contains three columns, i.e. gene name, microRNA name, and mirTarDANN prediction score. Predictions with positive scores are true predictions for miRNA;mRNA interactions, and vice versa. 


IV) For acdemic users, please feel free to use the code. For commercial users, please contact the authors.

V) The authors acknowledge the use of predictive results of miRanda, miRDB, PITA, and TargetScan in the application of mirTarDANN.



