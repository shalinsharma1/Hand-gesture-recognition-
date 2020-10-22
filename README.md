# Hand-gesture-recognition-
It will recognize the hand gesture like if you put your finger as one it will recognize it as one
This project is based on openCV.

I have used background subtraction model. OpenCV provides us with different back ground subtraction models I choose codebook ( no specific reason).What it does is it calibrates for some time to be exact for some frames.In which for all the images it acquires; it calculates the average and deviation of each pixel and accordingly designates boxes. For more information please refer a book.

     So at this stage we have removed the background and in the foreground we only have our hand. For those who are new to CV it is like a black and white image with only the hand as white.


  
   In the next part what we intend to do is recognise the gesture. Here we use Convex Hull to find the finger tips.Convex hull is basically the convex set enclosing the hand region.



     The red line bounding the hand is convex hull .Basically it’s a convex set ; means if we take any two points inside the red region and join them to form a line then the line entirely lies inside the set.




     The yellow dot is the defect point and there will be many such defect points i,e every valley has a defect point. Now depending upon the number of defect points we can calculate the number of fingers unfolded.



summary :-
The hand region extraction has been done using background substraction using codebook method.
For Tip points i have used convex hull 2 and for depth points convexity defects.
