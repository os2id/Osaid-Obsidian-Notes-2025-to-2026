No — they’re **three different technologies**, not one language.

- **HTML** = _structure/content_ (headings, paragraphs, buttons, forms)
    
- **CSS** = _style/design_ (colors, layout, fonts, responsive design)
    
- **JavaScript** = _behavior/logic_ (click actions, validation, fetching data, dynamic updates)


# ==HTML== (Text image)


### To start writing a code in HTML
![[Pasted image 20260111104051.png]]
We have an empty page 

just put [!] and hit enter:
![[Pasted image 20260111104125.png]]
![[Pasted image 20260111104148.png]]
Now we can put our code inside <,body><,/body>



## Headings in HTML
![[Pasted image 20260111093105.png]]
By [h1] code we can insert a heading 1 paragraph. We have headings to [h6]

![[Pasted image 20260111093241.png]]
![[Pasted image 20260111093314.png]]
We printed Hello my name is: Osaid



#### An example of heading 3
![[Pasted image 20260111101236.png]]
![[Pasted image 20260111101251.png]]
![[Pasted image 20260111101310.png]]
![[Pasted image 20260111101327.png]]


The whole code was written like that:






## Paragraph in HTML

<,p>Write text here<,/p>
![[Pasted image 20260111093803.png]]

![[Pasted image 20260111093607.png]]
![[Pasted image 20260111093825.png]]
The paragraph was [ <,p>In sha Allah I will be the best hacker in the world one day!<,/p> ]


### Bold text
1- <,b>Write text here<,/b>
![[Pasted image 20260111094246.png]]

Then we made it [ <,p>In sha <,b>Allah<,/b> I will be the best hacker in the world one day!<,/p> ]
To explain: ==Here we bolded== "Allah" 

Then ==we add a link to click== section if needed) a link about "Allah" from wikipedia. ((see ### Buttons (clickable text or image)))
[ <,a href="https://en.wikipedia.org/wiki/Allah"><,b>Allah<,/b><,/a> ]



2- ==Another way to bold the text using (strong)==
<,strong>Write text here<,/strong>
![[Pasted image 20260111094555.png]]
![[Pasted image 20260111095933.png]]
Here to explain: <,strong>best hacker<,/strong>

then we add a link inside the bolded


### Buttons (clickable text or image) in HTML
<,a href="put https link here">Inside here you can add text, image, or etc..<,/a>
![[Pasted image 20260111095517.png]]
![[Pasted image 20260111095838.png]]

## Break (to make a space between two texts) in HTML

1- We can use break
<,br>
![[Pasted image 20260111100715.png]]

For example
![[Pasted image 20260111100814.png]]
![[Pasted image 20260111100826.png]]




2- we can use paragraph
<,p>Write text here<,/p>
![[Pasted image 20260111100942.png]]


![[Pasted image 20260111100932.png]]
We got small text because it is paragraph function [p] and not a heading one. But I did it just to explain that we have two ways of separating texts

## To link an image or another file such as (css or javascript)
We have an image link problem:
![[Pasted image 20260114090119.png]]
Also if we used [ img src="./<,THE IMAGE NAME" alt="img" width="200" height="200"> ]  <,img src="./pngwing.com.png" alt="img" width="200" height="200"> ==IT WILL NOT WORK==, because [ ./ ] is used for forwarding ==SO TO SOLVE THE PROBLEM WE JUST PUT TWO DOTS== in order for the HTML code to look for it out // back


Here the file is out the HTML "folder" so we need to go back using [ ../ ] ==TWO DOTS NOT ONLE ONE== if we can forward we use only [ ./ ] ==ONE DOT==:
![[Pasted image 20260114090030.png]]
Here we used <,img src="../pngwing.com.png" alt="img" width="200" height="200">



## Image in HTML (non-clickable, clickable)

<!-- clickable -->
<,a href="page.html"><,img src="photo.jpg" alt=""><,/a>

<!-- non-clickable -->
<,img src="photo.jpg" alt="">

![[Pasted image 20260111102353.png]]
This is a clickable image also we specified the width and height of the image

<,a href="Put HTTPS link here">

    <,img src="Put the path of the image here // if we have it in the same folder of the code, we can just put the name of the image like the example we have in the screenshot" alt="img // photo " width="Number" height="Number">

    </a>

## Phishing using iframe

![[Pasted image 20260111103611.png]]
![[Pasted image 20260111103644.png]]
We embed the bing .com in our website (we can do a phishing attack using it)

### My code in phishing attack
![[Pasted image 20260111112449.png]]
![[Pasted image 20260111112504.png]]
   <,p>Click here this is a google link:<,a href="file:///G:/My%20Drive/ALL%20HTML,%20CSS,%20JAVASCRIPT%20CODES%20osaid/practice%20scripts.html"><,b>https://google.com<,/b><,/a><,/p>

To explain:
  <,p>Click here this is a google link:<,a href="put HTTPS link here"><,b>Write text here<,/b><,/a><,/p>

## Bullet points (nesting) in HTML

For this code
![[Pasted image 20260112092742.png]]


We have this result:
![[Pasted image 20260112092810.png]]
==BUT IN ORDER TO MAKE THE BULLET POINT IN A BETTER WAY, WE WILL USE== [ul] un-ordered list ==AND== [li] list

Here we used [ul] and [li]
![[Pasted image 20260112094037.png]]
![[Pasted image 20260112094054.png]]
![[Pasted image 20260112094117.png]]
See the difference between 1 and 2 bullets
![[Pasted image 20260112094212.png]]




![[Pasted image 20260112094821.png]]
![[Pasted image 20260112094836.png]]

![[Pasted image 20260112100506.png]]


Here he used [ol] which means ordered list, then he inserted list [li] with it, and then he inserted under the "Roadster 2" un-ordered list: 
![[Pasted image 20260112100540.png]]
We got this result from the upper code:
![[Pasted image 20260112100733.png]]




==THERE IS ALSO ANOTHER WAY==:
Here he used [ol] which means ordered list, then he inserted list [li] with it, and then he inserted under the "Roadster 2" an ordered list [ol] and inside the second ordered list [ol] he inserted other three lists [li]
![[Pasted image 20260112100839.png]]
We got this result from the upper code:
![[Pasted image 20260112101209.png]]




Just to see more example of listing:
![[Pasted image 20260112101258.png]]
We got this result:
![[Pasted image 20260112101345.png]]










## To solve HTML problem for writing inside 

![[Pasted image 20260112100057.png]]
![[Pasted image 20260112100115.png]]

==The solution of the upper screenshots (problem):==
![[Pasted image 20260112100225.png]]









# ==CSS **Cascading Style Sheets**== (coloring & styling)

## Center items in CSS 

[center] :
![[Pasted image 20260112102019.png]]
![[Pasted image 20260112102031.png]]
We can see here that we centered the photo using [center]

## Font (size and color)

[ font ] we can write on it [ <,font size=7 color="#FF1493">Write text here<,/font> ] OR <,font size=7 color="cyan">Write text here<,/font>

![[Pasted image 20260114083038.png]]
We can use different ratio colors from https://www.w3schools.com/cssref/css_colors.php :
![[Pasted image 20260114083121.png]]



## ==ANOTHER WAY OF COLORING AND STYLING EASILY== using style to change everything included inside the code:

[<,style>h1 { color = } ] :
![[Pasted image 20260114084149.png]]
So here because of the [ style ] we are making all h1s "red color":
![[Pasted image 20260114084251.png]]

Here we changed all h3 to purple color:
![[Pasted image 20260114084729.png]]
![[Pasted image 20260114084800.png]]


And here he did [ style ] but for "p" :
![[Pasted image 20260114084354.png]]
So here will change all paragraphs to red:
![[Pasted image 20260114084443.png]]

## ==USING STYLE== in CSS
![[Pasted image 20260114085213.png]]
















# ==JAVASCRIPT== (Funcionality of the website)

comments: 