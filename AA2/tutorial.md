Update the Configuration
=========================

In this activity, you will run the code for 3 generations where the first generation has 10 genomes and no hidden layers.


<img src= "https://media.slid.es/uploads/1525749/images/10589921/C78AA2.gif" width = "480" height = "220">



Follow the given steps to complete this activity:


1. Update the files


* Open the `config-feedforward.txt` file.


* Set the `pop_size` to `50`.

    `pop_size = 50`

*  Change the generations to `3` in the `p.run()` function.

    `winner = p.run(eval_fitness, 3)` 
                     
* Save and run the code to check the output.