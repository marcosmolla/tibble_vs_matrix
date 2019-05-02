# Tibble versus Matrix in an ABM context

Due to their large overhead, data.frames() are very slow when used with agent-based models. A much more efficient data type are matrices that come with a smaller overhead 

However, as the `tidyverse` keeps expanding a new data type might replace the matrix, namely the tibble. Here, I am benchmarking tibbles and matrices in an agent-based modelling context. I am using a very simple agent-based model that simulates the aging, death, and birth of a populatin that is comprised of three different types of individuals. 

## Results
For simulation runs <10e5 turns matrices are a lot faster when compared to tibbles. Interestingly, there is a strong shift back towards tibbles when simulations are run for much longer (10e6). Why? I cannot say yet. 
