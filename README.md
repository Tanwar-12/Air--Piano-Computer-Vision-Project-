# *Air-Piano-Computer-Vision-Project*



*Air Piano is a computer vision based project that allows you to play a virtual piano through hand-gesture.*

* First, the hand is detected using the the black color mask we created using the HSV scale. For this purpose, I chose to wear a pair of black gloves because detecting the skin color was comparitively tougher and would have deprived the project from generalisation.

* After the hand is detected, we draw a convex hull, to find the surrounding convex polygon. From this polygon we extract the finger-tips using the convexity defects function. The convexity defect function returns three points out of which our interest is only in the first set of points.(Read more through the links)
There is also a filter applied to get just the fingertips using the distance between the points, while you may also chose to use the angle between the fingers to achieve the same.

* The last part includes the PyAutoGUI library which allows you to do the keyboard operations depending on the co-ordintates of you hand movements(fingertips to be precise).
[Link to virtual piano keyboard](https://www.onlinepianist.com/virtual-piano)



## To run the project-
* Fork the project and clone it in your repo.
* Run the requirements.txt file as 
`pip install -r requirements.txt`
* Run the program and the streaming window will open.
* Then go to [Virtual Piano keyboard](https://www.onlinepianist.com/virtual-piano) and select that window. Now make finger-movements inside the white lines of your streaming window to play the piano!



