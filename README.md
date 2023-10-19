# 5LSM0-final-assignment
 Name : Jiaqi Ji Student ID: 1877879  
 CodaLab Username: Erastus  
 TU/e email address: j.ji@student.tue.nl  
 It seems that my teammate dropped the course long time ago. I am unable to contact my teammate.   
# About running the code:  
As stated in my paper, I used the data from the paper: Multi-weather city: Adverse weather stacking for autonomous driving,  which was cited in my paper.    
In order to acquire the data I used, please follow the instructions on authors' [github](https://github.com/vnmusat/multi-weather-city)  
Below is a brief insturction from [github](https://github.com/vnmusat/multi-weather-city):  
1. download the original cityscapes dataset.
2. download the cityscapes difference file: [link](https://drive.google.com/file/d/1AQ_zt6PLMV4myHXL5wSFkQwIahL8OPoV/view)  
3. extract the file and make sure the city-scapes difference folder and cityscapes folder are on the same level.
4. download the reconstruct_cond.py  
5. Use the following command in terminal   
     ```
    cd multi-weather-city
    python reconstruct_cond.py -cityscapes_path '/path/to/Cityscapes' -city_diff_path '/path/to/Cityscapes_difference' -multi_weather_city_path '/path/to/Cityscapes_multi_weather'
The argument ```-cityscapes_path```, is the path to the ```Cityscapes``` dataset that you just downloaded. The argument ```-city_diff_path```, is the path to the ```Cityscapes_difference``` folder that you just downloaded. The argument ```-multi_weather_city_path```, is the root path to where the original Cityscapes dataset will be resized and cropped, and to where all the other conditions will be reconstructed.

When it's done, there will be generated images under 7 conditions and original ones.

For full detailed process, please check the github of the author presented above.

Then it is necessary to compose the 3 conditions (rain, snow, night) into 3 train folders.
This is the combined dataset used in the assignment: [link](https://drive.google.com/file/d/1OJN8Fxggm_2eU44QXnSqYqlYeODsoRoe/view?usp=share_link)
Use this as a replacement for the original set.  
# Reference on coding process:
Dataset : [github](https://github.com/vnmusat/multi-weather-city)  
Some Coding part about the Deeplab structure: [github](https://github.com/bubbliiiing/deeplabv3-plus-pytorch)
