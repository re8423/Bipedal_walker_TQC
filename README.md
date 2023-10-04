# Bipedal_walker
This repo uses the Truncated Quantile Critics (TQC) to overcome overestimation bias in off policy learning for the bipedal walker environment (normal & hardcore).

* agent-code.ipynb
    >
    > This notebook contains all the code for the entire project, including code for the TQC model, training, as well as testing+recording of results. Simply installing the required packages and running the notebook from the top should replicate results.
    >
    >The entropy temperature value is auto-tuned. The total number of atoms M ∈ {5, 10, 15, 25, 35, 50} were explored and M = 25 was found to be optimal. Similarly, the number of critics N ∈ {1,2,3,4,5,10} as well as the number of dropped atoms d ∈ {0,1,2,3,4,5} were explored and N = 5 and d = 5 were optimal. Additionally, extensive experimentation with the hardcore environment found that adjusting the reward value such that failures are penalized less yielded better results, possibly due to the higher frequency of failure in the more difficult environment.
    >

Demo of the TQC model in the hardcore env after 990 episodes, with a reward of 330:
![Gifdemo](https://github.com/re8423/Bipedal_walker_TQC/blob/d962b38973a3097ce89ca686655ba4b28bf2753e/Results/agent-hardcore-video%2C%20episode%3D1000%2C%20score%3D312.gif)

<div class="img-with-text">
    <p>Below are the results of the TQC model in the normal env:</p>
    <a href="url"><img src="https://github.com/re8423/Bipedal_walker_TQC/blob/d962b38973a3097ce89ca686655ba4b28bf2753e/Results/normal.png" height="400" width="400" ></a>
</div>

<div class="img-with-text">
    <p>Below are the results of the TQC model in the hardcore env:</p>
    <a href="url"><img src="https://github.com/re8423/Bipedal_walker_TQC/blob/d962b38973a3097ce89ca686655ba4b28bf2753e/Results/hardcore.png" height="400" width="400" ></a>
</div>





