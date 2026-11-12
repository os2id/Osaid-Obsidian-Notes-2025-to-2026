https://drive.google.com/file/d/1lI5zTnbcICc69flm19gR2Bejy0cI9_Ql/view


## (The "Hello World!" code of Git)
![[Pasted image 20260422093314.png]]
[git --version] is to know if you installed git in the operating system and you should try the code inside the terminal of Visual Studio Code or Webstorm
![[Pasted image 20260424181354.png]]


## **To create a file that make you know who did the edit in the code**

![[Pasted image 20260422093801.png]]
 
[git config --global user.name "Osaid Alrabee" ]
[git config --global user.email "your-email@example.com"]

### **ChatGPT Explanation**
The benefit is that Git needs to know **who made each change** in the project.

Imagine you and your friends are working on the same project. Everyone edits files and saves changes using Git. Without a name and email, Git cannot clearly show who made which change.

So when you write:

git config --global user.name "Osaid"  
git config --global user.email "your-email@example.com"

you are basically telling Git:

> “When I save changes, write my name and email on those changes.”

This is useful because later, when you check the project history, you can see something like:

Osaid changed index.html yesterday  
Ahmed changed style.css today  
Sara fixed the login page

In Git, saving a change is called a **commit**. Each commit has an author.

So the main benefit is:

**It makes your work identifiable.**  
GitHub, GitLab, or Bitbucket can also use this email to connect your commits to your account.

For example, when you push your code to GitHub, GitHub may show:

Osaid committed 2 hours ago

instead of showing an unknown author.

Think of it like writing your name on an exam paper. The work is still the same, but the teacher needs to know who submitted it. Git does the same thing with your code changes.


## **To create a new Repos**itory

[git init]
![[Pasted image 20260424202305.png]]