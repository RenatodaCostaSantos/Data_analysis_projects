# Challenging topics in Physics


<p align="center">
  <img width="1000" height="500" src="equations.jpg">
</p>




NOTE: 

- THIS IS A WORK IN PROGRESS. 

- ONLY THE DATA SCRAPING PART IS FINISHED.

- I'M CURRENTLY BUSY WITH THE DATA EXPLORATION, CLEANING AND ANALYSIS WHICH WILL BE UPLOADED HERE SHORTLY.


Back to the project!

A couple of years ago, my long distance girlfriend at that time was studying for the University entrance exams when she asked me to teach her how to [compute the square root of decimal numbers](youtube.com/watch?v=v7AUT1TMxZM&t=8s). Instead of just sending her a video with my explanation, I decided to start a [channel on YouTube](https://www.youtube.com/channel/UCQJtnudYBb-nULKBjmkhTnw).

I made some other videos based on questions other friends asked me and some other random topics in Mathematics and Physics but I was always trying to think of a more sound way for choosing topics that would be really helpful for the students.

It turns out that the answer seems to always be in some kind of **data**. 

So, as a Brazilian physicist and knowing the difficulties and costs of high quality education in my country, I decided to build my first data science project with the intention to answer the following question:

**- Which topics/subtopics of Physics students in Brazil struggle the most?**

By answering this question I intend to be able to **select potential topics** and use this information to create new videos on my YouTube channel. 

The final goal is to target topics that are badly covered and give a valuable contribution to the educational system of my home country.

## Strategy

There are two ways I can think of how to approach this project:

1 - Look in the ministery of education website and search for open source data.

This would be the best approach but, unfortunately, the brazilian government is currently (September 2022) remodeling all the data due to the lack of anonimity on the so far, open available data.

Given that, I will use a second approach:

2.1 - Use the ministery of education information to collect all mandatory topics in Physics pertaining the brazilian school curriculum.

2.2 - Use the YouTube API to search for these topics on YouTube.

2.3 - Identify popular subtopics for a given topic.

2.4 - Analyse the data and identify potential subtopics where a contribution would be valuable for students.


## Main mandatory areas (topics) in the Brazilian school curriculum

Physics is usually divided in four big areas in the Brazilian school curriculum. They are:

1. Mecanica (Mechanics),

2. Eletromagnetismo (Electromagnestism),

3. Termodinamica (Thermodynamics),

4. Otica (Optics).

The main topic out of these four is Mechanics with usually [up to 44% of the questions](https://infoenem.com.br/questoes-de-fisica-enem/) of the university entrance exams being about some of its subtopics.

Given the amount of content in each of the topics, this project will focus only on subtopics of Mechanics. The approach taken here can be easily extended to all other areas.

### Subtopics in Mechanics

Mechanics is a huge branch of physics and can be divided into two main subtopics:
<br/><br/>

- Cinematica (kinematics), which deals with theh description of movements without taking into considerantion what is causing it.
<br/><br/>

The list of **subtopics** in the Brazilian education high school curriculum is the following:

 1. Movimento e Repouso
 2. Movimento Uniforme 
 3. Movimento Uniformente variado 
 4. Lançamento vertical para cima 
 5. Queda livre 
 6. Vetores / Lançamento oblíquo 
 7. Lançamento horizontal  
 8. Cinemática vetorial 
 9. Movimento Circular 
 10. Estática de um ponto material
 11. Centro de massa e equilíbrio
 12. Estática do corpo extenso.

<br/>

- Dinamica (dynamics), which explains the kinematic description by means of fundamental cause (force of gravity, the existence of a spring, etc).
<br/><br/>

The list of **subtopics** for the dynamics is given by:
<br/><br/>

13. Leis de Newton
14. Forças tração, normal e peso
15. Força elástica 
16. Força de atrito 
17. Trabalho e energia 
18. Impulso e quantidade de movimento 
19. Lei de Kepler 
20. Lei de gravitação Universal 
21. Satélite em órbitas circulares 
22. Velocidade de escape 
23. Aceleração da gravidade.
<br/><br/>

The Jupyter notebooks with the scrapped data, it's cleaning and exploration can be found in this project's folder.

# A guessing game

Before showing our analysis and conclusions let's take a minute to do some guessing about what we think we could expect given the available data.

Guessing the outcome has various benefits:

1. It forces us to use our intuition and think deeply about the problem we are investigating,

2. It can lead us to find some variables that could be engineered if machine learning is our final goal,

3. It helps on the cleaning and exploration analysis before we start deriving conclusions,

4. It makes us critical of our results beforehand.

For this project we have only 12 columns given by: 'video_id', 'title', 'description', 'tags', 'channel_id', 'duration', 'view_count', 'like_count', 'topic', 'subtopic','dificulty'.

My two guessess are:

1. Videos with length less than 10 minutes will have more views than longer videos.

2. Easy topics will be have more potential for new videos than hard ones (this is counter intuitive but my guess is that students struggle with simple topics and get stuck there. Even with high volume videos, it seems that many easy topics are still not covered in a more intuitive way).

       
   




# Intermission!

The follow up data analysis and conclusions will be posted here soon!

