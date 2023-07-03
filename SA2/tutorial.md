Stop the Car
==============

In this activity, you will stop the car when it goes off the track.


<img src= "https://media.slid.es/uploads/1525749/images/10589195/sa2__1_.gif" width = "480" height = "220">


Follow the given steps to complete this activity:


1. Preprocess the video

* Open the main.py file.

* Define the function to find the `coordinates` and `dimensions` of the car to extract the 4 end points.

    `x = car.x`

    `y = car.y`

    `width = car.width`

    `height = car.height`


    `if(checkPixel(x,y) or checkPixel(x+width, y) or checkPixel(x, y+height) or checkPixel(x+width, y+height)):`

      `return True`
`

* Define a function to check if any end point of the car is black.

    `def checkPixel(x, y):`

        `global screen`

        `try:`

            `color = screen.get_at((x, y))`

        `except:`

            `return 1`

        `if(color == (163,171,160,255)):`

            `return 0`

        `return 1`


* Increase the genome Count and reposition the car if pixel color of any of its end points is black.


    `if(checkOutOfBounds(player)):`

        `player.x = 60`

        `player.y = 300`

        `angle =0`

        `genomeCount = genomeCount +1`

        `break`


* Save and run the code to check the output.
