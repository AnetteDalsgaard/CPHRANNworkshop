CPHRANN Workshop, Session 2
================

Prototyping an Artificial Neural Network in Base R
--------------------------------------------------

You will find a simple Artifical Neural Network implemented in base R [here](../R/session_1_prototyping_an_artificial_neural_network_in_base_R.R) (This script is also in the directory `/R` of your RStudio session)

*Your task is to, make the script run and find and tune the hyperparameters `n_hidden`, `epochs` and `epsilon` to get a working model*

<details><summary>When you have the script running and a working model, click here to see suggested hyperparameters</summary>

-   `n_hidden = 4` (The number of hidden neurons)
-   `epochs = 100` (The number of training cycles)
-   `epsilon = 0.01` (The learning rate, i.e. size of steps towards a better model)

Ok, so this was not particularly straight forward, it doesn't scale and writing complicated models this way would be challenging, to say the least. Let us take a break and when we come back from the break, let us see if there is a better way.

</details>

When you are looking at the code, it might be a good idea to keep this visualisation in mind:

![alt text](../lectures/figures/ann_04.png)
