# curl-opencv
Using curl to read images from URL in opencv program. 

# Compile
In order to compile the program, you must install 'curl' on the system. Choose any one the following way to install curl in ubuntu:    
1. Use the following command to install curl in ubuntu    
  `sudo apt-get install curl`    
2. Download and install curl from the following repository    
   `https://github.com/curl/curl`    

After installing curl, use the following command to compile the program.
g++ curl-opencv.cpp -o main `pkg-config --cflags --libs opencv` -lcurl

# Example    
./main URL

Try:    
./main https://cdn.pixabay.com/photo/2017/02/13/08/54/brain-2062057_960_720.jpg   

It should display the following image on the screen.
![alt text](https://raw.githubusercontent.com/2vin/curl-opencv/master/data/brain.jpg)
