# IMC-git101
<h1>Generae ssh key ad add to Gtithub</h1>
1.use command "$ssh-keygen" <br/>
2.copy data in id_rsa.pub <br/>
3.setting ssh key on github <br/>

<h1>Testing SSH connection</h1>
use command "$SSh -T git@github.com" <br/>

<h1>Add remote</h1>
use command "$git remote add [NICKNAME] [Remote url]" <br/>

<h1>Remove remote</h1>
use command "$git rm [NICKNAME]" <br/>

<h1>Rename remote</h1>
use command "$git rename [OLD NICKNAME] [NEW NICKNAME]" <br/>

#Working with branch

Each branach point to a commit
- after commit it look like  below.

                  ==========<br/>
                  = Master =<br/>
                  ========== <br/>
                       |	<br/>
                       V<br/>
======    ======    ======<br/>
= C1 = <- = C2 = <- = C3 =<br/>
======    ======    ======<br/>
   |         |         |<br/>
   V	     V         V<br/>
======== ========  ========<br/>
=Tree 1= =Tree 2=  =Tree 3=<br/>
======== ========  ========<br/>

It make pointer of commit same pointer
----------------------------------------

Create new branch
command : git branch [BRANCH NAME]

Switch branch
command : git checkout [BRANCH NAME]

Delete branch
command : git branch -d [BRANCH NAME]

Show all branch
command : git branch
=======
******************************************************
*                          Remote Repository                                      *
******************************************************
1) git push => copy source code from Local to Remote Repository
    push to remote => used syntax "git push [NICKNAME] [BRANCH]"
    Fetch and Merge => use syntax "git pull [NICKNAME] [BRANCH]"
2) git clone => combine "git init" + "git remote" + "git pull" 
3) git pull => pull source code from Remote Repository to Local
    "git pull" make sequence as fetch then merge
    => git fetch [NICKNAME] only pull source code, not auto merge
    => git merge [BRANCH]  
	=> git rebase [BRANCH]  

Commit --> $commit -m "Your Messsage"
Status --> $git status
Lift Cycle of File Status | ( Untracked -> Unmodified -> Modified -> Staged)
Try to reset --> $git resert HEAD <file>
Remove files --> $rm <file>
Remove files (git) --> $git rm <file>
Remove files (git cache) --> $git rm --cached <file>
Help Command --> $git help <COMMAND>
Move files --> $git MV <NAME> <NEW NAME>

