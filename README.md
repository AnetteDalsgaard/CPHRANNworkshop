Introduction to Artificial Neural Networks in R using Keras/TensorFlow
================

This is the GitHub repository for the [CopenhagenR useR meetup March 7th 2019](https://www.meetup.com/CopenhagenR-useR-Group/events/258482768/)

Getting started
---------------

### Cloud Solution

[RStudio](https://www.rstudio.com/) has kindly sponsored 100 [m5.large (3.1 GHz, 2CPU, 8GB ram) EC2 AWS instances](https://aws.amazon.com/ec2/instance-types/). These have been preinstalled with the following R-packages: `keras`, `tidyverse`, `broom` and `cowplot`. At the workshop, you will be given instructions on how to access an instance.

### Local Solution

<details><summary>If you plan to use your own laptop, please click here *before* the workshop</summary>

Due to time constraints, please make sure, that you have successfully completed the following steps:

1.  Install the latest versions of `R` for [Linux](https://mirrors.dotsrc.org/cran/bin/linux/), [Mac](https://mirrors.dotsrc.org/cran/bin/macosx/) or [Windows](https://mirrors.dotsrc.org/cran/bin/windows/)
2.  Install the latest verstion of [`RStudio`](https://www.rstudio.com/products/rstudio/download/#download)
3.  Open `RStudio` and run the following commands one-by-one at the console:

``` r
install.packages('tidyverse')
install.packages('broom')
install.packages('cowplot')
install.packages('devtools')
devtools::install_github('rstudio/keras')
library('keras')
install_keras()
```

Then you can check your installation like so:

``` r
library('tidyverse')
library('keras')
mnist = dataset_mnist()
mnist %>% pluck('train') %>% pluck('x') %>% dim
dim(mnist$train$x)
```

Congratulations! That's it! Now you're ready for the workshop! </details>

At the Workshop
---------------

### Schedule

-   17.30 - 17.50 Session 1, part I: Lecture - Introduction to Neural Networks \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/01_intro_to_ANNs/lecture/01_introduction_to_neural_networks.html)\] (MathJax not supported by GitHub html preview. To view slides, [download](https://raw.githubusercontent.com/leonjessen/CPHRANNworkshop/master/01_intro_to_ANNs/lecture/01_introduction_to_neural_networks.html) and open with your browser)
-   17.50 - 18.15 Session 1, part II: Exercise - Simple Artificial Neural Network in Base R \[[Link](https://github.com/leonjessen/CPHRANNworkshop/blob/master/01_intro_to_ANNs/exercises/01_exercises.md)\]
-   18.15 - 18.30 Break
-   18.30 - 18.35 Session 2, part I: Lecture - Introduction to TensorFlow \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/02_intro_to_TF/lecture/02_introduction_to_tensorflow.html#1)\]
-   18.35 - 18.50 Session 2, part II: Exercise - TensorFlow Playground \[[Link](https://github.com/leonjessen/CPHRANNworkshop/blob/master/02_intro_to_TF/exercises/02_tensorflow_playground.md)\]
-   18.50 - 18.55 Session 2, part III: Lecture - Introduction to TensorFlow Continued \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/02_intro_to_TF/lecture/02_introduction_to_tensorflow_continued.html#1)\]
-   18.55 - 19.15 Session 2, part IV: Exercise - Building a simple neural network using Keras and Tensorflow \[[Link](https://github.com/leonjessen/CPHRANNworkshop/blob/master/02_intro_to_TF/exercises/02_simple_keras_ann.md)\]
-   19.15 - 19.30 Break
-   19.30 - 19.45 Session 3, part I: Lecture - Introduction to Model Validation \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/03_intro_to_model_validation/lecture/03_intro_to_model_validation.html)\]
-   19.45 - 20.15 Session 3, part II: Exercise - Regression on diamonds with Cross Validation \[[Link](https://github.com/leonjessen/CPHRANNworkshop/blob/master/03_intro_to_model_validation/exercises/03_diamond_regr_with_cv.md)\]
-   20.15 - 20.30 Session 4, Workshop Wrap Up and Q&A \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/04_wrap_up/lecture/04_wrap_up.html)\]

Resources
---------

### Web

-   [R API to TensorFlow](https://tensorflow.rstudio.com/)
-   [R API to Keras](https://keras.rstudio.com/)
-   [Learning Resources](https://tensorflow.rstudio.com/learn/resources.html)
-   [RStudio Community](https://community.rstudio.com/)
-   [RStudio Cloud](https://rstudio.cloud/)

### Cheat Sheets

-   [Deep Learning with Keras Cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/keras.pdf)
-   [RStudio IDE](https://github.com/rstudio/cheatsheets/raw/master/rstudio-ide.pdf)
-   [Data Import with readr](https://github.com/rstudio/cheatsheets/raw/master/data-import.pdf)
-   [Data Transformation with dplyr](https://github.com/rstudio/cheatsheets/raw/master/data-transformation.pdf)
-   [Data Visualization with ggplot2](https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf)

### Books

-   [Deep Learning with R](https://www.manning.com/books/deep-learning-with-r)
-   [Free: Deep Learning book](https://www.deeplearningbook.org/)
-   [Free: R for Data Science by Garrett Grolemund and Hadley Wickham](https://r4ds.had.co.nz/)
-   [ModernDive - An Introduction to Statistical and Data Sciences via R](https://moderndive.com/)
