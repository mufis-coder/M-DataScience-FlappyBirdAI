# Flappy Bird AI

Game ini terinspirasi dari tutorial [Tech With Tim](https://www.youtube.com/watch?v=MMxFDaIOHsE&list=PLzMcBGfZo4-lwGZWXz5Qgta_YNX3_vLS2&ab_channel=TechWithTim). Perbedaan code yang saya buat dan tutorial tersebut adalah: pipa yang saya buat, bergerak ke atas dan ke bawah. Hal ini, saya lakukan agar model AI yang ada pada game bisa belajar lebih keras untuk menjalankan "bird" dalam melewati rintangan. Selain itu, perbedaan lainnya adalah input pada model AI pada game ini ada empat.

Code input: 

```
output = nets[x].activate((bird.y, abs(bird.y-pipes[pipe_ind].height), 
			abs(bird.y - pipes[pipe_ind].bottom), pipes[pipe_ind].x, bird.x))
```

Penjelasan input tersebut adalah: 

- ```bird.y``` adalah: posisi "bird" terhadap y-axis (vertikal)
- ```abs(bird.y-pipes[pipe_ind].height)``` adalah: 


Demo game:

![alt text](https://github.com/mufis-coder/M-DataScience-FlappyBirdAI/blob/main/doc/demo-game.gif) <br />