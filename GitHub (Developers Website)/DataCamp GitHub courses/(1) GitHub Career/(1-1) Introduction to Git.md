Directory = folder

Study sections:
1- Useful terminal comands ([pwd], [ls])
2- Changing directory ([cd])
3- Checking Git version ([git --version])
4- Repos (what is Git repo, benefits of repos, Creating and checking status of the repo [git init <,name of the repo>] and [git status], create a repo to an existing directory, Tracking if all files are being tracked inside the directory by using [git status] in the repo, Avoid Git Nested repositories).
5- Staging and committing files ( packaging and delivering files, Making a commit using [-m] in [git commit -m "<, something>]).
6- viewing the version history ( )



![[Pasted image 20260429012226.png]]

![[Pasted image 20260429012236.png]]

![[Pasted image 20260429012257.png]]


![[Pasted image 20260429012442.png]]
Here he was explaining that let us say for example the new release of our code has a bug, we can revert to the older version until we finish from fixing the bug so costumers do not be mad because of lack performance.



![[Pasted image 20260429012639.png]]


![[Pasted image 20260429012755.png]]


![[Pasted image 20260429012834.png]]
Directory = folder

## ==## Useful terminal comands ([pwd], [ls])==

![[Pasted image 20260429012902.png]]
[pwd] : checks our location, where we are in?
[ls] : lists the files we have inside the directory we are in


## ==## Changing directory ([cd])==
![[Pasted image 20260429013113.png]]
[cd] : changes / goes to the directory or place we specified
[pwd] : checks our location, where we are in?


## ==## Checking Git version ([git --version])==

![[Pasted image 20260429013543.png]]
[git --version] : checks our Git version installed in our device

## ==##Practice (1-3 study sections)==

Datacamp exercise 1 explanation:
![[Pasted image 20260429013816.png]]

My solution exercise 1:
![[Pasted image 20260429014013.png]]
Done! correct answer



Datacamp exercise 2 explanation:
![[Pasted image 20260429014111.png]]

My solution exercise 2:
![[Pasted image 20260429014132.png]]
Done! correct answer




## ==## Repos (what is Git repo, benefits of repos, Creating and checking status of the repo [git init <,name of the repo>] and [git status], create a repo to an existing directory, Tracking if all files are being tracked inside the directory by using [git status] in the repo, Avoid Git Nested repositories)==

![[Pasted image 20260429014511.png]]

![[Pasted image 20260429014601.png]]

### ### Creating and checking status of the repo [git init <,name of the repo>] and [git status]
![[Pasted image 20260429014829.png]]
[git init <,name of the repo>] : Creates a new repo
[cd <,repo or folder name>] : goes to the repo 
[git status] : to check if we initialized/created the repo successfully

### ### Create a repo to an existing directory
![[Pasted image 20260429015750.png]]

### ### Tracking if all files are being tracked inside the directory by using [git status] in the repo
![[Pasted image 20260429015719.png]]


### ### Avoid Git Nested repositories
![[Pasted image 20260429020117.png]]
==Nested repos means putting a repo inside a repo, here Git will be confused which repo it should commit to==


### ### Practice (Repos)
Datacamp exercise 1 explanation:
![[Pasted image 20260429020503.png]]

My solution exercise 1:
![[Pasted image 20260429020541.png]]
Done! correct answer


Datacamp exercise 2 explanation:
![[Pasted image 20260429020724.png]]

My solution exercise 2:
![[Pasted image 20260429020733.png]]
Done! correct answer



Datacamp exercise 3 explanation:
![[Pasted image 20260429020858.png]]

My solution exercise 3:
![[Pasted image 20260429020916.png]]
Done! correct answer




Datacamp exercise 4 explanation:
![[Pasted image 20260429021007.png]]

My solution exercise 4:
![[Pasted image 20260429021029.png]]
Done! correct answer

## ==## Staging and committing files ( packaging and delivering files, Making a commit using [-m] in [git commit -m "<, something>])==

![[Pasted image 20260429021304.png]]

The staging area is used by Git to track changes to files within your current directory and sub-directories: 
![[Pasted image 20260429021406.png]]
Staging is like packaging an email

committing is like delivering the email to the costumer


![[Pasted image 20260429021724.png]]
[git add <,file name>.md]
[git add .] : The (dot) here means all like the star symbol ( * ) in python. Here it will commit all modified files in the directory or sub-directory we are currently located in (inside it : the directory)


### ### Making a commit using [-m] in [git commit -m "<, something>]
![[Pasted image 20260429022334.png]]
[git commit -m "<, something>]


### ### Practice (Staging and committing files)
Datacamp exercise 1 explanation:
![[Pasted image 20260429022544.png]]

My solution exercise 1:
![[Pasted image 20260429022846.png]]
Done! correct answer


Datacamp exercise 2 explanation:
![[Pasted image 20260429022923.png]]

My solution exercise 2:
![[Pasted image 20260429023041.png]]
Done! correct answer




Datacamp exercise 3 explanation:
![[Pasted image 20260429023201.png]]

My solution exercise 3:
![[Pasted image 20260429023139.png]]
Done! correct answer


Datacamp exercise 4 explanation:
![[Pasted image 20260429023402.png]]

My solution exercise 4:
![[Pasted image 20260429023422.png]]
Done! correct answer



