# Malicious-URLs-Detection

###Problem Statement
In this case study, we address the detection of malicious URLs as a multi-class classification problem. In this case study, we classify the raw URLs into different class types such as benign or safe URL, phishing URL, malware URL, or defacement URL.

As we know machine learning algorithms only support numeric inputs so we will create lexical numeric features from input URLs. So the input to machine learning algorithms will be the numeric lexical features rather than actual raw URLs. If you don't know about lexical features you can refer to [this](https://stackoverflow.com/questions/33282094/differences-between-lexical-features-and-orthographic-features-in-nlp) discussion about a lexical feature in StackOverflow.

So, in this case study, we will be using three well-known boosting machine learning classifiers namely XGBoost, Light GBM, Gradient Boosting Machines.
