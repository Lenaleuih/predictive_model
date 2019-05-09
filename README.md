# Prediction

Many universities have a problem with students over-enrolling in courses at the beginning of semester and then dropping most of them as the make decisions about which classes to attend. This makes it difficult to plan for the semester and allocate resources. However, schools don't want to restrict the choice of their students.One solution is to create predictions of which students are likley to drop out of which courses and use these predictions to inform semester planning. 

## use cases and application

* discuss different uses for prediction algorithms in education
* discuss the theory behind the CART, C4.5 and C5 classification algorithms
* Construct classification models to predict student dropout and state validation metrics for the model
* Compare classification models on appropriate metrics

## setup and installations

In order to generate our models we will need several packages. The first package you should install is [caret](https://cran.r-project.org/web/packages/caret/index.html). (https://topepo.github.io/caret/train-models-by-tag.html)(https://cran.r-project.org/web/packages/caret/vignettes/caret.pdf)

There are many prediction packages available and they all have slightly different syntax. caret is a package that brings all the different algorithms under one hood using the same syntax. 

We will also be accessing an algorithm from the [Weka suite](https://www.cs.waikato.ac.nz/~ml/weka/). Weka is a collection of machine learning algorithms that have been implemented in Java and made freely available by the University of Waikato in New Zealand. To access these algorithms you will need to first install both the [Java Runtime Environment (JRE) and Java Development Kit](http://www.oracle.com/technetwork/java/javase/downloads/jre9-downloads-3848532.html) on your machine. You can then then install the [RWeka](https://cran.r-project.org/web/packages/RWeka/index.html) package within R.

(Issue 1: failure to install RWeka/RWekajars, paste "sudo R CMD javareconf" into terminal and try to install again)

**Weka requires Java and Java causes problems. If you cannot install Java and make Weka work, please follow the alternative instructions at line 121**

The last package you will need is [C50](https://cran.r-project.org/web/packages/C50/index.html)

## how does it work
*We will modelling student data using three flavors of tree algorithm: CART, C4.5 and C5.0.
*We will be using these algorithms to attempt to predict which students drop out of courses.  

*we will be using the tree algorithms to build models of which students are likely to drop out of which classes. 


## references

[Adhatrao, K., Gaykar, A., Dhawan, A., Jha, R., & Honrao, V. (2013). Predicting Students’ Performance Using ID3 and C4. 5 Classification Algorithms. International Journal of Data Mining & Knowledge Management Process, 3(5).](https://arxiv.org/ftp/arxiv/papers/1310/1310.2071.pdf)

[Brooks, C. & Thompson, C. (2017). Predictive modelling in teaching and learning. In The Handbook of Learning Analytics. SOLAR: Vancouver, BC](https://solaresearch.org/hla-17/hla17-chapter5/)
