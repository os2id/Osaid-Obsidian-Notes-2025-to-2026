Chapter Matplotlib (1-3):
1- Matplotlib (The Mother of Visualization: [matplotlib] we studied scatter and plot)

2- Histogram ([bins=#], [plt.clf()])

3- Customization (Axis Labels using [plt.xlabel("")] OR [plt.ylabel("")], Labelling the Title in out plot data using [plt.title("")], To make the Y-axis of the plot data starts from zero using Ticks 1 and 2 [plt.yticks(<,you put a list here>)] OR [plt.xticks(<,you put a list here>)], What we Took in the practice section: Labelling all of x and y axis and the title -- Ticks 1 and 2 -- Doubling the size of the Circles -- We used Grid and in the question itself they used [plt.text] to put the text of India and China in the plot )



Chapter Dictionaries & Pandas (4-#):
4-
5-
6-
7-

# # Chapter 1-3

## ==## Matplotlib==

![[Pasted image 20260502232159.png]]

![[Pasted image 20260502232247.png]]

![[Pasted image 20260502232415.png]]



### ### The Mother of Visualization: [matplotlib]
Inside matplotlib we have: plot and scatter
![[Pasted image 20260502232719.png]]
[plt.plot(<,Horizontal Axis>, <,Vertical Axis>)]
(year, pop) : Year is Horizontal Axis and pop is Vertical Axis

[plt.show()] Here it displays the data:
![[Pasted image 20260502233028.png]]


#### #### Scatter plot 
![[Pasted image 20260502233204.png]]
[plt.scatter(<,Horizontal Axis>, <,Vertical Axis>)]
(year, pop) : Year is Horizontal Axis and pop is Vertical Axis

[plt.show()] Here it displays the data:
![[Pasted image 20260502233028.png]]


### ### Practice (Matplotlib)
Datacamp exercise 1 explanation:
![[Pasted image 20260502233536.png]]

My solution exercise 1:
![[Pasted image 20260502234318.png]]
Done! correct answer







Datacamp exercise 2 explanation:
![[Pasted image 20260502234357.png]]

My solution exercise 2:
![[Pasted image 20260502234623.png]]
Done! correct answer









Datacamp exercise 3 explanation:
![[Pasted image 20260502234655.png]]

My solution exercise 3:
![[Pasted image 20260503003447.png]]
Done! correct answer







Datacamp exercise 4 explanation:
![[Pasted image 20260503003607.png]]

My solution exercise 4:
![[Pasted image 20260503003726.png]]
Done! correct answer







Datacamp exercise 5 explanation:
![[Pasted image 20260503003750.png]]

My solution exercise 5:
![[Pasted image 20260503004009.png]]
Done! correct answer


## ==## Histogram==

![[Pasted image 20260503004606.png]]



Here we cam specify many things in the Histogram but the most important ones are the first two:
![[Pasted image 20260503004648.png]]

Here it is divided into three bins, using [bins=3] :
![[Pasted image 20260503004840.png]]


![[Pasted image 20260503004926.png]]


#### #### ChatGPT explanation about [plt.clf()] means **clear the current figure**.

In Matplotlib, it removes everything from the current plot area, such as:

- scatter points
- lines
- labels
- title
- axes content

It is useful when you want to create a **new clean plot** after making another plot.

Example:

```
import matplotlib.pyplot as pltplt.scatter(pop, life_exp)plt.show()plt.clf()   # clears the previous plotplt.plot(year, pop)plt.show()
```

Without `plt.clf()`, sometimes the old plot and the new plot may appear together or affect each other.

Simple meaning:

```
plt.clf()
```

= “Clear the figure and start fresh.”



### ### practice (Histogram)
Datacamp exercise 1 explanation  ==plt.hist()== :
![[Pasted image 20260503005520.png]]

My solution exercise 1:
![[Pasted image 20260503005529.png]]
Done! correct answer







Datacamp exercise 2 explanation ==bins=  ==:
![[Pasted image 20260503010006.png]]

My solution exercise 2:
Bins 5 Histogram:![[Pasted image 20260503010511.png]]

Bins 20 Histogram:
![[Pasted image 20260503010721.png]]
Done! correct answer








Datacamp exercise 3 explanation ==Histogram & bins & plt.clf== :


My solution exercise 3:
life_exp with 15 bins Histogram:
![[Pasted image 20260503011013.png]]

life_exp1950 with 15 bins Histogram:
![[Pasted image 20260503011117.png]]
Done! correct answer




Datacamp exercise 4 explanation ==which is better for a teacher/grader== :
![[Pasted image 20260503011302.png]]

My solution exercise 4:
![[Pasted image 20260503011302.png]]
Done! correct answer





Datacamp exercise 5 explanation ==which is better to select for seeing is longer answers mean higher grades== :
![[Pasted image 20260503011553.png]]

My solution exercise 5:
![[Pasted image 20260503011554.png]]
Done! correct answer


## ==## Customization==
![[Pasted image 20260503013237.png]]



Here we can see that the data is showing good but there is no many details for the person who is seeing it for the first time, so how can we solve the problem? This is why we will dive more into Customization section:
![[Pasted image 20260503013331.png]]


### ### Axis Labels using [plt.xlabel("")] OR [plt.ylabel("")] 
Here we can see that we annotated:
![[Pasted image 20260503013542.png]]



### ### Labelling the Title in out plot data using [plt.title("")]
Here we can see that we showed the Title (World Population Projections) in our plot data:
![[Pasted image 20260503014045.png]]


### ### To make the Y-axis of the plot data starts from zero using Ticks 1 and 2 [plt.yticks(<,you put a list here>)] OR [plt.xticks(<,you put a list here>)]
Here we 
![[Pasted image 20260503014449.png]]


Here we want to make it clearer for the reader with adding (B) which stands for (Billion) so we have to use (Ticks 2) and it should be the same length as for Ticks 1 list length. Here he changed the list of (0, 2, 4, etc..) to be (0, 2B, 4B, etc..) so the reader can understand the Data easier:
![[Pasted image 20260503014818.png]]


### ### Add More Historical Data in Our Previous Data
The Data was like that:
![[Pasted image 20260503015403.png]]

He wrote this:
![[Pasted image 20260503015221.png]]
To explain what he did:
year = <, A List> + <, The List he wants to add the data on, in our case (year) is the name of the list>
pop = <, A List> + <, The List he wants to add the data on, in our case (pop) is the name of the list>>

The Result:
![[Pasted image 20260503015208.png]]
![[Pasted image 20260503015720.png]]





### ### Practice (Customization) 
Datacamp exercise 1 explanation ==Label x, Label y, Label Title== :
![[Pasted image 20260503020216.png]]

My solution exercise 1:
![[Pasted image 20260503020310.png]]
Done! correct answer






Datacamp exercise 2 explanation ==Ticks 1 and 2== :
![[Pasted image 20260503020338.png]]

My solution exercise 2:
![[Pasted image 20260503021344.png]]
Done! correct answer







Datacamp exercise 3 explanation ==Doubling the size of the Circles== :
![[Pasted image 20260503021528.png]]
![[Pasted image 20260503021537.png]]



My solution exercise 3:
It is now smaller:
![[Pasted image 20260503022355.png]]
Done! correct answer


Datacamp exercise 4 explanation ==Changed the color and used alpha== :
![[Pasted image 20260503022532.png]]
![[Pasted image 20260503022611.png]]
My solution exercise 4:
![[Pasted image 20260503023409.png]]
Done! correct answer





Datacamp exercise 5 explanation ==We used Grid and in the question itself they used [plt.text] to put the text of India and China in the plot== :
![[Pasted image 20260503023752.png]]
![[Pasted image 20260503023759.png]]
My solution exercise 5:
![[Pasted image 20260503023814.png]]
Done! correct answer







Datacamp exercise 6 explanation ==== :
![[Pasted image 20260503024240.png]]
![[Pasted image 20260503024246.png]]
My solution exercise 6:
![[Pasted image 20260503024409.png]]
Done! correct answer




# # Chapter 4-7



