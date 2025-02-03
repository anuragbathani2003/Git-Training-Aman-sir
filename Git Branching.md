
## Branch Creation 

to create the branch follow the bellow command 

	git branch <new branch name>

	example
	git branch feature1
to see all current branches follow the bellow command

	git branch

![](https://i.imgur.com/ANutpvb.png)

## Create a Branch with Checkout

to create a branch and want to point the head to the newly created branch use -b with git branch command

	git checkout -b <branch name>

![](https://i.imgur.com/5QwLY0M.png)


## Under Standing the WorkFlow

		#Creating some dummy files and commiting them
		echo "<h1>This is my website</h1>" > index.html
		git add index.html
		git commit -m "Created index.html"
		echo "h1, h2, h3 { margin-bottom: 15px; }" > style.css

		git add style.css
		
		git commit -m "Created style.css"
		
		#Checking out the logs
		git log --all --graph
	

![](https://i.imgur.com/4KbwC7W.png)


### creating a new branch and checkout that branch

![](https://i.imgur.com/Yud3LJV.png)

### add new feature in the repo

![](https://i.imgur.com/T14NjcY.png)


![](https://i.imgur.com/kBdYpVo.png)

### switch a branch from feature1 to main


![](https://i.imgur.com/ORAPTIu.png)


### fix a bug in a branch and commit it

![](https://i.imgur.com/X1CZNre.png)



![](https://i.imgur.com/ibdeZnG.png)

### sync with github



![](https://i.imgur.com/yOJ1mqv.png)


### merge a branch to main



![](https://i.imgur.com/YjBqhVB.png)



![](https://i.imgur.com/D7WqWLy.png)

# creating merge conflict

Make a GIt Repo Named "git-merge-test"
clone it in local machine

### Commands
	echo "this is some content to mess with" > merge.txt
	git add merge.txt
	git commit -m "we are commiting the inital content"


![](https://i.imgur.com/Pc1JTBG.png)


## Make a new branch and perform commit

### Commands

	```bash
	git checkout -b new_branch_to_merge_later
	echo "totally different content to merge later" > merge.txt
	git add .
	git commit -m "edited the content of merge.txt to cause a conflict"
	```

![](https://i.imgur.com/H9fVIMU.png)


### do the same thing on main but diffrent content

Create a merge.txt in main and write some different thing on it

### commands

	```bash
	git checkout main
	echo "content to append" >> merge.txt
	git add .
	git commit -m "appended content to merge.txt"
	```

![](https://i.imgur.com/IXBi3Vf.png)


### now merge the new_branch_to_merge_later in main

#### commands
	git merge new_branch_to_merge_later

![](https://i.imgur.com/ZHJGu92.png)


	git status

![](https://i.imgur.com/hEkFdvS.png)

Check the status what is the conflict

in vs code the pop up open called merge conflict select accept the changes and commit 

	git log --all --graph

![](https://i.imgur.com/I7XYmTq.png)

## Branch Precticing through Git visulizer

![](https://i.imgur.com/uBDNISR.png)
