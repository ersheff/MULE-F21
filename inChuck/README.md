# [inChuck - Stephen David Beck](https://sdbeck.blog/music/inchuck/)

Welcome to inChuck. You perform inChuck by adding melodic "processes"
to the system, indicating which process, how many times it should be played,
and in what register.
  
[Performance Video](https://www.youtube.com/embed/-ZrmajoMxcE)
  
<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/-ZrmajoMxcE" frameborder="0" allowfullscreen="true"> </iframe>
</figure>
  
### Launching inChuck
Open a command prompt (Terminal on Mac, Command Prompt on Windows). Change directory to the location of the inChuck score folder, e.g.  
  
```cd ~/Desktop/MULE-F21/inChuck/score```  
  
Enter the command:  
  
```chuck inChuckCode.ck --loop &```
  
### Performing inChuck

To add a process to the piece, type:  
   
```chuck + x:y:z```  
   
where:
 x is the process number (1 - 19),
 y is the number of repetions (8 is default), and
 z is the octave (2 - 7, 4 is middle register and default).
   
Example: "chuck + 3:10:5" plays process #3 ten times an octave above middle C.
   
Play the processes in sequence. Start at process 1. You are encouraged to 
repeat a process, but you should not go backwards. Focus on one process for
between 30-60 seconds.
   
Take your time and listen to what others are doing. Make sure you sustain the
ensemble's sound density. Most importantly, have fun.
When you have reached process #19 and are done, type "chuck --kill".
   
If you are the pulse, start now by typing:  
   
```chuck + pulse*```

[Score](inchuck_score.pdf)

### To-Dos
- Establish command-line performance process for Windows