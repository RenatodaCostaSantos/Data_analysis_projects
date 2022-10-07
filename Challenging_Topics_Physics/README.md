# Potential topics in Physics


<p align="center">
  <img width="1000" height="500" src="equations.jpg">
</p>

What do you mean by potential topics, you might ask. Please read below to find out.

A couple of years ago, my long-distance girlfriend at that time was studying for the University entrance exams when she asked me to teach her how to [compute the square root of decimal numbers](youtube.com/watch?v=v7AUT1TMxZM&t=8s). Instead of just sending her a video with my explanation, I decided to start a [channel on YouTube](https://www.youtube.com/channel/UCQJtnudYBb-nULKBjmkhTnw).

I made some other videos based on questions other friends asked me and some other random topics in Mathematics and Physics but I was always trying to think of a more sound way to choose topics that would be really helpful to the students.

So, as a Brazilian physicist and knowing the difficulties and costs of high-quality education in my country, I decided to build my first data analysis project with the intention to answer the following question:

**- Which topics/subtopics of Physics students in Brazil struggle with the most?**

By answering this question I intend to be able to **select potential topics** and use this information to create new videos on my YouTube channel. 

Potential topics are those that are badly covered by YouTubers, but searched often by students. By identifying a few of them  I can use this information to create videos for my youtube channel and contribute more effectively to the educational system of my home country.

## Strategy

There are two ways I can think of how to approach this project:

1 - Look in the ministry of education website and search for open source data.

This would be the best approach but, unfortunately, the Brazilian government is currently (September 2022) remodeling all the data due to the lack of anonymity on the so far, openly available data.

Given that, I will use a second approach:

2.1 - Use the ministry of education information to collect all mandatory topics in Physics pertaining to the Brazilian school curriculum.

2.2 - Use the YouTube API to search for these topics on YouTube.

2.3 - Identify popular subtopics for a given topic.

2.4 - Analyse the data and identify potential subtopics where a contribution would be valuable for students.


## Main mandatory areas (topics) in the Brazilian school curriculum

Physics is usually divided into four big areas in the Brazilian school curriculum. They are:

1. Mecanica (Mechanics),

2. Eletromagnetismo (Electromagnestism),

3. Termodinamica (Thermodynamics),

4. Otica (Optics).

The main topic out of these four is Mechanics with usually [up to 44% of the questions](https://infoenem.com.br/questoes-de-fisica-enem/) of the university entrance exams being about some of its subtopics.

Given the amount of content in each of the topics, this project will focus only on subtopics of Mechanics. The approach taken here can be easily extended to all other areas.

### Subtopics in Mechanics

Mechanics is a huge branch of physics and can be divided into two main subtopics:
<br/><br/>

- Cinematica (kinematics), which deals with the description of movements without taking into consideration what is causing it.
<br/><br/>

The list of **subtopics** in the Brazilian education high school curriculum is the following:

 1. Movimento e Repouso (Rest and motion)
 2. Movimento Uniforme (Uniform motion)
 3. Movimento Uniformente variado (Motion with constant acceleration)
 4. Lançamento vertical para cima (Upward vertical launch)
 5. Queda livre (Free fall)
 6. Vetores / Lançamento oblíquo (Vectors / Projectile launch)
 7. Lançamento horizontal  (Horizontal launch)
 8. Cinemática vetorial (Vector kinematics)
 9. Movimento Circular (Circular motion)
 10. Estática de um ponto material (Static of a material point)
 11. Centro de massa e equilíbrio (Center of mass and balance)
 12. Estática do corpo extenso (Statics of a rigid body).

<br/>

- Dinamica (dynamics), which explains the kinematic description by means of a fundamental cause (force of gravity, the presence of a spring, etc).
<br/><br/>

The list of **subtopics** for the dynamics is given by:
<br/><br/>

13. Leis de Newton (Newton's law)
14. Forças tração, normal e peso (Tension, normal, and weight forces)
15. Força elástica (Elastic force)
16. Força de atrito (Friction force)
17. Trabalho e energia (Mechanical work and energy)
18. Impulso e quantidade de movimento (Impulse and momentum)
19. Lei de Kepler (Kepler's law)
20. Lei de gravitação Universal (Law of universal gravitation)
21. Satélite em órbitas circulares (Satellites in circular orbits)
22. Velocidade de escape (Escape velocity)
23. Aceleração da gravidade (Gravitational acceleration).
<br/><br/>

# Our goals

1. Are short videos watched more often than longer ones?
<br/><br/>
2. Which class of topics has more views? Hard, easy or moderate topics?
<br/><br/>
3. Which specific topics are worth investing on video production for my youtube channel?


# A guessing game

Before showing our analysis and conclusions let's take a minute to do some guessing about what we think we could expect given the available data.

Guessing the outcome has various benefits:

1. It forces us to use our intuition and think deeply about the problem we are investigating,

2. It can lead us to find some variables that could be engineered and improve the quality of our analysis,

3. It helps with the cleaning and exploration analysis before we start deriving conclusions,

4. It makes us critical of our results beforehand.


My guesses are:
<br/><br/>
**Guess for question 1:** Longer videos have **fewer views** than shorter ones.

While making videos for youtube I remember always becoming a bit anxious to force the length of the video to be under 8 minutes precisely because of this guess. My intuition is that students lack attention in general and want to learn things fast.
<br/><br/>
**Guess for question 2:**  **Easy** topics will have, on average, more views than **hard** topics. However, I expect **hard** topics to be better covered than **easy** ones.

The first part of the answer would happen because of the struggles students face when start learning physics. They seem to get stuck right in the beginning.

Even though easy topics would have more views I expect to find a reasonable amount of easy topics that are not well covered.

I believe people that make videos for youtube intuitively think that hard topics should get more attention, which will lead to a higher number of successful videos for hard topics.

**Guess for question 3:** I can't think of a reasonable answer for this one. We will leave it to the data.


# Data analysis

More precise and technical analysis and answers for the questions below can be found in the jupyter nootebooks. 

We try to use a more intuitive, however less precise, approach below. 

## Are shorter videos watched more often than longer ones?

The graph below shows that, contrary to our guess, longer videos seem to have more views than shorter ones. 

Actually, the graph suggests that videos with the time duration that fall into the 8 to 12 minutes or higher than 14 minutes are usually watched more often. 

This means no need to be anxious to keep the videos under 8 minutes when recording physics videos for youtube.


<p align="center" width="100%">
    <img width="80%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/positive_corr.png?raw=true"> 
</p>

## Are easy topics watched more often than hard ones?

Even though a bar plot tends to lose a lot of information, it can give us an indication of the answer in this case. 

As we see below, moderate and easy topics have more views, on average, than hard ones. This indicates that the first part of our guess is correct. 
<p align="center" width="100%">
    <img width="60%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/avg_view2_diff.png?raw=true"> 
</p>


In our analysis, we defined the score of videos as the like-to-view ratio. That means a video with a number of likes closer to the number of views will have a high score. That's how we classify successful videos here.

The bar plot below shows exactly that. Easy videos seem to have, on average, a lower score. This gives an indication that easy topics could have more potential than hard and moderate ones. 

<p align="center" width="100%">
    <img width="60%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/avg_score_diff.png?raw=true"> 
</p>

However, as the barplot loses a lot of information, a definite answer can only be found by looking at each subtopic separately. 

## Which subtopics should we invest in video production?

We can identify three main subtopics to focus our attention on video production by looking at the number of very high-quality videos per subtopic:

<p align="center" width="100%">
    <img width="100%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/high_quality_videos_per.png?raw=true"> 
</p>


We choose the three subtopics with the lowest percentage of very high-quality videos as having a higher potential to invest. They are given by:

1.  **Forças de tração normal e peso (Tension, normal, and weight forces)**

A more detailed analysis shows that this subtopic is highly searched by students and has the lowest percentage of very high-quality videos. Definitely our winner in this analysis.

2. **Aceleração da gravidade (Gravitational acceleration)**

This one has the third-lowest score, but the second-highest number of views. Since it is more searched by students, it will increase the chance of our video being viewed more often, even though there are more very high-quality videos on this subtopic.

3. **Centro de massa e equilíbrio (Center of mass and balance)**

It has the second-lowest score, but the third-highest number of views among the three videos we chose to invest our efforts in video production. It is a hard topic and usually less searched by students, and I would invest time in it only after putting effort into the ones above.


# Summary


When making Physics videos for youtube in Brazilian Portuguese, I suggest the following:

- **Focus on videos where the time duration stays in the interval of 8 to 20 minutes.**

Make videos covering the following subtopics in the following order:

1 - **Forças de tração normal e peso (Tension, normal, and weight forces - best subtopic)**;

2 - **Aceleração da gravidade (Gravitational acceleration - second best)**;

3 - **Centro de massa e equilíbrio (Center of mass and balance - third best)**.


**Connect with me on [LinkedIn](https://www.linkedin.com/in/renato-costa-b937851b3/)**.






