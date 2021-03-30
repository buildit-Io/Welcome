**NAVIGATE ME**

* [Welcome to buildit.Io](#welcome-to-buildit)
	* [GitHub For the New Dev](#github-for-the-new-Dev)


# Welcome to BuildIT

## GitHub For the New Dev

For the lost, newbie, developer who is trying to work in a team that employs GitHub:copyright: as a collaboration tool but was thrown to the deep end.

To begin working on this project, you first need to have downloaded GIT for your system 


![](https://git-scm.com/images/logo@2x.png)

#### Links 

[GIT for Windows](https://git-scm.com/download/win)

[GIT for Mac](https://git-scm.com/download/mac)

[GIT for Linux/Unix Systems](https://git-scm.com/download/linux)

>*The following assumes knowledge in the use of an Integrated Development Environment(IDE) or any text editor with an in-built terminal. We recommend either [Visual Studio](https://visualstudio.microsoft.com/), [Visual Studio Code](https://code.visualstudio.com/) or [any JetBrains IDE](https://www.jetbrains.com/products/#type=ide). **VIM is not recommended for new developers.** If you don't know what VIM is then ignore the warning. The reason why an IDE is recommended is because of the strong integration that IDEs have with GIT, which makes your coding journey feel less of a pain, especially when collaborating on a software project as a team*


##### After Installing GIT...

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

	__*Bite-sized Branching for the New Dev*__

	*Branching is the main way to **NOT MUCK UP** your project. Think about branching as creating a 
copy of the current main branch without downloading the main project into your local system. This is important in the later stages of the software project when we want to* `push` *changes to the project (**or in layperson terms, we want to modify the project when a developer has made some changes to the copy of the original program on his local computer and wishes to change the actual original program hosted on GitHub:copyright:**). Branches are made so that when a developer does a* `push` *operation from the developer's local computer, it ends up as a* `merge` *request for the* `main` *branch of the repository - which first requires an approval - rather then acting on the* `main` *branch itself. This is an additional layer of checks and balances employed to ensure that changes made to the actual program are ones that have already been approved by the owner of the* `main` *branch. As small changes in one part of the code may very quickly make the entire program **FAIL**, this is also a good method to ensure that the evolution of a project can be tracked through a history of* `push` *requests that can be seen by the owner of the repository.*

6. Navigate to the `amplifyIo` folder by entering `cd amplifyIo` or `cd path-to-amplifyIo-on-your-computer` into the Terminal
7. Enter `git branch`
8. If you are coming from 3i , you will notice the following result
