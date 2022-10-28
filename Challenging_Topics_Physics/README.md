# Potential topics in Physics


<p align="center">
  <img width="1000" height="500" src="equations.jpg">
</p>

You may wonder what do I mean by "potential topics". Allow me to explain.

A couple of years ago, my long-distance girlfriend at that time was studying for the University entrance exams when she asked me to teach her how to [compute the square root of decimal numbers](youtube.com/watch?v=v7AUT1TMxZM&t=8s). Instead of just sending her a video with my explanation, I decided to start a [channel on YouTube](https://www.youtube.com/channel/UCQJtnudYBb-nULKBjmkhTnw).

I made some other videos based on questions other friends asked me, and some other random topics in Mathematics and Physics. I was always trying to think of a more comprehensive way to choose topics, however, that would be broadly helpful to scholars and students.

So, as a Brazilian physicist, and knowing the difficulties and costs of high-quality education in my country, I decided to build my first data analysis project with the intention to answer the following question:

**- Which topics/subtopics of Physics do students in Brazil struggle with the most?**

Identifying these topics will guide me to create YouTube content that will contribute more effectively to the education system in my home country.

## Strategy

I considered two ways to approach this project:

1 - Look at the ministry of education website and search for open source data.

This would be the best approach but, unfortunately, the Brazilian government is currently (September 2022) remodeling all the data due to the lack of anonymity on the data.

Given that, I will use a second approach:

2.1 - Use the ministry of education information to collect all mandatory topics in Physics pertaining to the Brazilian school curriculum.

2.2 - Use the YouTube API to search for these topics on YouTube.

2.3 - Identify popular subtopics for a given topic.

2.4 - Analyse the data and identify potential subtopics where a contribution would be valuable for students.


## Main mandatory areas (topics) in the Brazilian school curriculum

Physics is usually divided into four main areas in the Brazilian school curriculum. They are:

1. Mecanica (Mechanics),

2. Eletromagnetismo (Electromagnestism),

3. Termodinamica (Thermodynamics),

4. Otica (Optics).

The most important of these four is Mechanics with usually [up to 44% of the questions](https://infoenem.com.br/questoes-de-fisica-enem/) of the university entrance exams being about some of its subtopics.

Given the amount of content in each of the topics, this project will focus only on subtopics of Mechanics. The approach taken here can easily be extended to all other areas.

### Subtopics in Mechanics

Mechanics is a huge branch of physics and can be divided into two main subtopics:
<br/><br/>

- Cinematica (kinematics), which deals with the description of movements without considering its cause.
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
 10. Estática de um ponto material (Statics of a material point)
 11. Centro de massa e equilíbrio (Center of mass and balance)
 12. Estática do corpo extenso (Statics of a rigid body).

<br/>

- Dinamica (dynamics), which explains the kinematic description by means of a fundamental cause (force of gravity, the presence of a spring, etc).
<br/><br/>

The list of **subtopics** for the dynamics is given by:
<br/><br/>

13. Leis de Newton (Newton's laws)
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

#Goals

1. Are short videos watched more often than longer ones?
<br/><br/>
2. Which class of topics has more views? Hard, easy or moderate topics?
<br/><br/>
3. Which specific topics will be of most value to scholars?


# A guessing game

Before showing up my analysis and conclusions, let's consider what might be expected, given the available data.

Attempting to predict the outcome has various benefits:

1. It forces us to use our intuition and think deeply about the problem we are investigating,

2. It can lead us to find some variables that could be engineered to improve the quality of our analysis,

3. It helps with the cleaning and exploratory analysis before we start deriving conclusions,

4. It makes us critical of our results beforehand.


My guesses are:
<br/><br/>
**Question 1:** Longer videos have **fewer views** than shorter ones.

While making videos for YouTube I remember always becoming a bit anxious to force the length of the video to be under 8 minutes precisely because of this assumption. My intuition is that students lack attention in general and want to learn things fast.
<br/><br/>
**Question 2:**  **Easy** topics will have, on average, more views than **hard** topics. However, I expect **hard** topics to be better covered than **easy** ones.

The first part of the answer would happen because of the struggles students face when starting to learn physics. They seem to get stuck right in the beginning.

Even though easy topics would have more views I expect to find a reasonable amount of easy topics that are not well covered.

I believe that people who make videos for YouTube intuitively think that "hard" topics should get more attention, which will lead to a higher number of successful videos for hard topics.

**Question 3:** I can't think of a reasonable answer for this one. We will leave it to the data.


# Data analysis

More precise and technical analyses and answers for the questions below can be found in the Jupyter notebooks. 

Below I describe a more intuitive, though less precise approach.

## Are shorter videos watched more often than longer ones?

The graph showss that, contrary to my assumption, longer videos have more views than shorter ones. 

Actually, the graph suggests that videos with the time duration that fall into the 8 to 12 minutes or above 14 minutes are usually watched more often. 

This means no need to be anxious to keep the videos under 8 minutes when recording physics videos for YouTube.


<p align="center" width="100%">
    <img width="80%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/positive_corr.png?raw=true"> 
</p>

## Are easy topics watched more often than hard ones?

Even though a bar plot tends to lose a lot of information, it can give us an indication of the answer in this case. 

As we see below, moderate and easy topics have more views, on average, than hard ones. This indicates that the first part of my hypothesis is correct. 
<p align="center" width="100%">
    <img width="60%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/avg_view2_diff.png?raw=true"> 
</p>


In my analysis, I defined the score of videos as the likes-to-views ratio. That is, if the number of likes is similar to the number of views, the score will be high.

The bar plot illustrates the finding that "easy" topic videos have a lower score, on average, than difficult ones. This gives an indication that "easy" topics could have more potential than "hard" and "moderate" ones. 

<p align="center" width="100%">
    <img width="60%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/avg_score_diff.png?raw=true"> 
</p>

However, as the barplot loses a lot of information, a definite answer can only be found by looking at each subtopic separately. 

## In which subtopics should I invest my time?

In order to identify the three main subtopics with greatest potential, I looked at the number of high-scoring videos per subtopic:

<p align="center" width="100%">
    <img width="100%" src="https://github.com/RenatodaCostaSantos/Portfolio/blob/main/Challenging_Topics_Physics/images/high_quality_videos_per.png?raw=true"> 
</p>


The three subtopics with the lowest percentage of high-scoring videos were selected for new YouTube videos. They are:

1.  **Forças de tração normal e peso (Tension, normal, and weight forces)**

A more detailed analysis shows that this subtopic is highly searched by students and has the lowest percentage of high-scoring videos. Definitely our winner in this analysis!

2. **Aceleração da gravidade (Gravitational acceleration)**

Although this subtopic has the third-lowest score, it has the second-highest number of views meaning that videos on this topic have greater potential to be of benefit to scholars.

3. **Centro de massa e equilíbrio (Center of mass and balance)**

While this topic has the second-lowest score, it also has a lower number of views than topics 1 and 2. Thus, I determined that scholars do not seek out this topic as often as they do for the previous two; so this shall be the third topic on which I invest my time.

# Summary


When making Physics videos for YouTube in Brazilian Portuguese, I suggest the following:

- **Aim to produce videos of 8 to 20 minutes duration.**

Focus attention on these subtopics, in the following order:

1 - **Forças de tração normal e peso (Tension, normal, and weight forces)**;

2 - **Aceleração da gravidade (Gravitational acceleration)**;

3 - **Centro de massa e equilíbrio (Center of mass and balance)**.


**Connect with me on [LinkedIn](https://www.linkedin.com/in/renato-costa-b937851b3/)**.






