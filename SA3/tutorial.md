Control the Car Movement
========================

In this activity, you will create neural networks for each genome to check the fitness and move the car to the left or right.


<img src= "https://media.slid.es/uploads/1525749/images/10589181/sa3__1_.gif" width = "480" height = "220">



Follow the given steps to complete this activity:


1. Move the car


* Open the main.py file.


* Creating neural network for each genome using current genome and configuration


    `net = neat.nn.FeedForwardNetwork.create(genome, config)`


* Move the car straight forward
 
    `forward = True`

    `change = 0`


* Feed input to the neural network and store output with fitness value

    `output = net.activate((player.x,player.y))`


* Change the direction of the car to left or right depending on the fitness value of the output


    `if output[0] > 0.65:`

        `change = 3`

          `if output[1] > 0.65:`

              `change = -3`
             
* Save and run the code to check the output.
