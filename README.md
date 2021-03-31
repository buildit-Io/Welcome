# BuildIT.io

> The BuildIT.Io self-help/intro/new dev page. Everything that aren't related to the specific projects will fall under this repo

## **NAVIGATE ME**
* [Top](#buildit.io)
	* [Welcome to buildIT](#welcome-to-buildit)
	* [GitHub For the New Dev](#github-for-the-new-Dev)
		* [Git Download Links](#links)
		* [Using GIT](#why-branching)	 
		* [Branching for New Devs](#why-branching)	 
	* [Using GIT on IDEs](#using-git-for-ides)
		* [Terminal?](#finding-the-terminal)
		* [CLI GIT](#git-on-terminal)
		* [IDE GIT](#git-on-the-toolbar)	 	

## Welcome to BuildIT.io

BuildIT is a wannabe Big-Tech-esque Company that focuses on taking up software projects and tagging monetary value to them. We want to build a company for New Developers, focusing on helping them to gain market exposure by embarking on our projects and breaking them into the market. 

At the same time, we aim to build a strong developer core that is multi-faceted in their skill sets and have a genuine interest in solving issues. We don't just want you for being able to describe Djikstra's Algorithm to us. We want ***you***.

Engineering is in BuilIT's DNA. We are primarily a software company and we use programming to solve issues and provide solutions. We are not glorified wrapper kings. We try to be as KISS as possible with our products and we try to provide solutions that are bespoke to client needs. As BuildIT progresses, the hope is that it will one day be a full-scale engineering company that can accept a wide scale of issues and provide practical and cost-efficient solutions.

As part of BuildIT's effort to focus on the New Age Developer, we have come up with a few simple tutorials that most Senior Developers already have exposure to through their many years in the field. However, this information is likely too annoying and/or simplistic to teach new developers entering the field. 

Here at BuildIT, we try to shy away from conventional "Baptisms of Fire" and focus instead on buidling up the ability and confidence of our New Developers. We at BuildIT want to create something sustainable and practical for the new age economy, and we believe that at the core, we should do away with toxic coding environments that puts anybody down simply because they don't know how to write code the way somebody wants them to.

If you're new to working on a BuildIT project, or you're a new employee, we at BuildIT would like to extend our warmest greetings to you and we really hope that you have a blast at learning how to code in a team and being part of a bigger machinery!

Else, we hope you enjoy the tutorials all the same!

> Traditions are like cliches. They are everywhere. They may sometimes even be correct, but often they are justified by nothing except constant repetition. 

## GitHub For the New Dev

For the lost, newbie, developer who is trying to work in a team that employs GitHub:copyright: as a collaboration tool but was thrown to the deep end.

To begin working on this project, you first need to have downloaded GIT for your system 

\
![](https://git-scm.com/images/logo@2x.png)


### Links 

[GIT for Windows](https://git-scm.com/download/win)

[GIT for Mac](https://git-scm.com/download/mac)

[GIT for Linux/Unix Systems](https://git-scm.com/download/linux)

>*The following assumes knowledge in the use of an Integrated Development Environment(IDE) or any text editor with an in-built terminal. We recommend either [Visual Studio](https://visualstudio.microsoft.com/), [Visual Studio Code](https://code.visualstudio.com/) or [any JetBrains IDE](https://www.jetbrains.com/products/#type=ide). **VIM is not recommended for collaboration.** If you don't know what VIM is then ignore the warning. The reason why an IDE is recommended is because of the strong integration that IDEs have with GIT, which makes your coding journey feel less of a pain, especially when collaborating on a software project as a team*


### After Installing GIT...

1. Open up Terminal on your IDE/Text Editor.

2. Navigate to the folder you wish to download this repository to.
	1. Use `cd your-folder-name` or `cd path-to-the-folder` to navigate to the desired directory
	
	2. Use `mkdir new-folder` to create a new folder in that directory
3. Choose the following
    1. run `git clone -b your-branch-name  https://github.com/buildit-Io/amplifyIo.git` if a branch has already been created for you by the owner 
    2. run `git clone https://github.com/buildit-Io/amplifyIo.git`
    
    	*(If option 3i was chosen, the following steps are not necessary and you can actually begin working on the development of the project unless your branch was removed by the owner or you want to create your own sub branch)*

4. After completing the cloning process, type `ls` in the terminal. You should now see the `amplifyIo` folder in the directory

5. Before the next step, a little trivia for the new developers:

	>__Bite-sized Branching for the New Dev__
	>
	>	*Branching is the main way to **NOT MUCK UP** your project. Think about branching as creating a 
copy of the current main branch without downloading the main project into your local system. This is important in the later stages of the software project when we want to* `push` *changes to the project (**or in layperson terms, we want to modify the project when a developer has made some changes to the copy of the original program on his local computer and wishes to change the actual original program hosted on GitHub:copyright:**). Branches are made so that when a developer does a* `push` *operation from the developer's local computer, it ends up as a* `merge` *request for the* `main` *branch of the repository - which first requires an approval - rather then acting on the* `main` *branch itself. This is an additional layer of checks and balances employed to ensure that changes made to the actual program are ones that have already been approved by the owner of the* `main` *branch. As small changes in one part of the code may very quickly make the entire program **FAIL**, this is also a good method to ensure that the evolution of a project can be tracked through a history of* `push` *requests that can be seen by the owner of the repository.*

6. Navigate to the `amplifyIo` folder by entering `cd amplifyIo` or `cd path-to-amplifyIo-on-your-computer` into the Terminal
7. Enter `git branch`
8. If you are coming from 3i , you will notice the following result,
	
	``` 
	*your-branch
	```
	
   else,
   	
	```
	*master
	```
	**OR**
	
	``` 
	*main
	```
	
9. To make a new branch from any parent branch, enter `git branch your-new-branch parent-branch`. if you see `*master` or `main` on the previous step, `git branch your-new-branch` will suffice
10. To switch between branches, enter `git checkout the-branch-you-wish-to-navigate-to`.
11. Typically, at this stage, you're going to make changes to the code in your branch. After this, you need to do the following:
	1. `git commit -m "write a meaningful comment about your changes"`
	2. `git push origin your-branch` if you're pushing to the main branch of the repository or `git push branch-to-push-changes-to your-branch`. 
12. And you're done! You can now work effectively as part of a Software Team
**BONUS**
13. Let's say you want to update your repository to match the parent-branch, this is what you do
	1. `git fetch branch-to-update-from` -> this command shows you all the files that are different 
	2. `git pull` this will attempt to merge all the files by allowing you to first compare the differences
	3. `git merge origin/branch-to-merge` -> this effectively writes all the changes from the parent-branch into the current-branch

Usually, IDEs allow you to pull and accept changes manually. This is covered more in the specific IDE docs or the [quickguide](#using-git-on-ides) below!

#### Why Branching?

Branching is pretty cool because it allows you to manage multiple versions of your work without having to worry that altering anything on your current code, will break your original program. That's because all the changes are only happening inside the branch (this is written into the feature of GIT) and the only way to make changes to any other branch would be to `git branch other-branch` and then make changes on the code while on that branch. Changes made and saved on the other branch is also **NOT LOST** when you switch branches. Lastly, to finalise changes, the `git push` request must be approved and then `git merge` with the original branch. There is no other way. Cool huh!

Here's a simple diagram to illustrate:

\
![](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)


Using this diagram as a reference, you could even branch out from the your own branch, creating a branch of a branch, and write changes to your branch only when you are ready to do so. All this can be done by using the same concepts as laid out in the [walk-thorugh](#github-for-the-new-Dev) above, without the explicit need to keep multiple copies of the same code in your computer everytime you save your work. And can you imagine having to save a copy of your work everytime you need to make changes, and then go through debugging hell just to find out what changes you made broke your program (We've all been there) ? With the `git commit` -> `git push` -> approval -> `git merge` cycle, you can do away with doing extra work just to make sure you don't do anything stupid. Now that's pretty amazing.

Well that's the end of the walk-through. Hope you enjoyed it!

## Using GIT on IDEs

IDEs are amazing tools for developers. It's the glorified toolbox equivalent for any developer. BuildIT recommends the following IDEs - [Visual Studio](https://visualstudio.microsoft.com/), [Visual Studio Code](https://code.visualstudio.com/) or [any JetBrains IDE](https://www.jetbrains.com/products/#type=ide) - because they have been tried and tested in the market for a long time now. 

This section is focused on using GIT with IDEs and not any of the specific functionalities of the IDEs themselves. This is because IDEs are all different and have their own seperate toolchains and features which will really become useful depending on the use cases of each specific task/project. If anything, the specific feature that needs to be used for the IDE should be highlighted in the official README or documentation of the tasks/project itself. **THIS IS NOT A Q AND A PAGE**. We do this solely for the sanity of all developers in BuildIT and to help foster a sense of independent learning within the company walls. 

Let's get to it.

### Finding the terminal

If you haven't read the [GitHub For the New Dev](#github-for-the-new-Dev) section of this README, we highly suggest you do. If not, you'll just be lost in this section.

GIT is a software that runs on a terminal. The terminal is basically a command line interface, which looks a little something like this:
```
Computer-238177:~ user$ 
```
and can be found at the bottom of the IDE when you first start the IDE.

If not, you can follow this *general* steps to activate the terminal
1. Naviagate to the top bar.
2. Go through the drop down menus of each segement. 
	* For Visual Studio, you can find this under *Tools* > *Command Line* > *Developer Command Prompt*. 
	* For Visual Studio Code, you can find this under *View* > *Terminal*
	* For Jetbrain IDEs, you can find this under *View* > *Tool Windows* > *Terminal*
4. Click on the option to activate the Terminal
5. You will see the terminal pop up in the screen

### GIT on terminal

Once you've activated the terminal, you can use the same `git` commands on the terminal in the IDE to use GIT. **ALWAYS REMEMBER TO BE IN THE CORRECT DIRECTORY**. The last thing you want to be doing is making git commands when you're not in the correct directory

### GIT on the toolbar

Most IDEs have the *Git* drop down on the toolbar. This basically works the same way as command line instructions. The only difference is that the error messages and certain processes that would have been easier to just key in the `git` command is now expressed in a visual form instead of simply just on the command line. 
