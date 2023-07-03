Load and Configure the Neural Network
===============================


In this activity, you will load and configure the neural network and create generation of genomes.



<img src= "https://media.slid.es/uploads/1525749/images/10589206/sa1__1_.png" width = "480" height = "220">



Follow the given steps to complete this activity:


1. Load and configure the network


* Open the main.py file.


* Load the NEAT configuration file

    `config = neat.config.Config(neat.DefaultGenome, neat.DefaultReproduction,neat.DefaultSpeciesSet, neat.DefaultStagnation,'config-feedforward.txt')`


* Create a population for the configuration

    `p = neat.Population(config)`


*   Define a fitness function to display genome count , generation count and length of each generation

    `global angle, gen, forward, change`

    `gen = gen+1`

    `genomeCount = 1`


* Load the NEAT configuration file

    `for gid, genome in generation:`

      `infoText = font.render('Generation :'+ str(gen)+  ' genomecount: '+str(genomeCount)+"/"+str(len(generation)) , True, (255,255,0))`


* Run the fitness function for 10 generations

    `winner = p.run(eval_fitness,10)`

         
* Save and run the code to check the output.