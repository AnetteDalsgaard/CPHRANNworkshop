Introduction to Artificial Neural Networks in R using Keras/TensorFlow
================

This is the GitHub repository for the [CopenhagenR useR meetup March 7th 2019](https://www.meetup.com/CopenhagenR-useR-Group/events/258482768/)

Getting started
---------------

### Cloud Solution

[RStudio](https://www.rstudio.com/) has kindly sponsored 100 [m5.large (3.1 GHz, 2CPU, 8GB ram) EC2 AWS instances](https://aws.amazon.com/ec2/instance-types/). These have been preinstalled with the following R-packages: `keras`, `tidyverse`, `broom`, `cowplot` and a few others. At the workshop, you will be given instructions on how to access an instance. If you are new to instances, just think of it as running RStudio in the browser.

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

Workshop Schedule
-----------------

*Since we only have 3 hours, we are on a bit of a tight schedule, so please follow the timing. This GitHub repo will remain active after the workshop, so you can revisit the workshop material.*

**Session 1**

-   17.30 - 17.50 (20 min) Lecture: *Introduction to Workshop* \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/lectures/session_1_introduction_to_workshop.html)\]
-   17.50 - 18.15 (25 min) Exercise: *Prototyping an Artificial Neural Network in Base R* \[[Link](exercises/session_1_prototyping_an_artificial_neural_network_in_base_R.md)\]

-   18.15 - 18.30 (15 min) *Break*

**Session 2**

-   18.30 - 18.35 (5 min) Lecture: *Introduction to TensorFlow* \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/lectures/session_2_introduction_to_tensorflow.html)\]

-   18.35 - 18.50 (25 min) Exercise: *The TensorFlow Playground* \[[Link](exercises/session_2_the_tensorflow_playground.md)\]

-   18.50 - 18.55 (5 min) Lecture: *Introduction to TensorFlow Continued* \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/lectures/session_2_introduction_to_tensorflow_continued.html)\]

-   18.55 - 19.15 (20 min) Exercise: *Building a simple neural network using Keras and Tensorflow* \[[Link](exercises/session_2_building_a_simple_neural_network_using_keras_and_tensorflow.md)\]

-   19.15 - 19.30 (15 min) *Break*

**Session 3**

-   19.30 - 19.45 (15 min) Lecture: *Introduction to Model Validation* \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/lectures/session_3_introduction_to_model_validation.html)\]

-   19.45 - 20.15 (30 min) Exercise: *Regression on `diamonds` with Cross Validation* \[[Link](exercises/session_3_regression_on_diamonds_with_cross_validation.md)\]

**Session 4**

-   20.15 - 20.30 (15 min) Lecture: *Workshop Wrap Up and Q&A* \[[slides](http://htmlpreview.github.io/?https://github.com/leonjessen/CPHRANNworkshop/blob/master/lectures/session_4_workshop_wrapup_and_QandA.html)\]

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
