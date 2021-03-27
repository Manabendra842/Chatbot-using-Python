# Chatbot-using-Python

![Screenshot (69)](https://user-images.githubusercontent.com/70123028/112720814-ae41a900-8f26-11eb-968e-8377f6db0b46.png)

**ATTENTION**

A common error SOLVED

If you are using Python 3.8 , download the previous version

Go to CMD

pip install chatterbot==1.0.4

This will work and everything is installed 

You will probably get an error after some time, where it says

File "C:\Python38\lib\site-packages\sqlalchemy\util\compat.py

", line 264, in <module>

    time_func = time.clock

AttributeError: module 'time' has no attribute 'clock'

This is because time.clock() function was removed in  Py 3.8. 

Go to the search  bar and then paste the location given right above the last line of error

It will look something like this :   C:\Python38\lib\site-packages\sqlalchemy\util\compat.py


Open file with IDLE or whatever editor you have 


Then , go to line 264  in that . It would be written 

time_func = time.clock()


Instead of this change, it to 

time.perf_counter()


Save the file and now run it. It will work
