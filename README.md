# Modul 9 Reflection
**Salma Kurnia Dewi (2206026681)** 

## 1.2 Understanding how it works 
What happened when you run the program?
<img src= "img/howdy.png">
Based on the image, the output 'hey hey' are printed before the 'howdy!' and 'done!'. This happened because the code ```!("Salma's Computer: hey hey!")``` is placed in the main thread outside of aynchronous task so it can run without waiting for the ```executor.run()``` to be executed first. 
Meanwhile, the code ```println!("Salma's Computer: howdy!")``` and ```println!("Salma's Computer: done!") are placed inside the asynchronous task and spawned with the code ```spawner.spawn(async{...}), where those codes can only run the ```executer.run()``` is executed first.  