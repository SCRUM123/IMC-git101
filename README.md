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

                  ==========
                  = Master =
                  ========== 
                       |	
                       V
======    ======    ======
= C1 = <- = C2 = <- = C3 =
======    ======    ======
   |         |         |
   V	     V         V
======== ========  ========
=Tree 1= =Tree 2=  =Tree 3=
======== ========  ========

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

Commit --> $commit -m "Your Messsage"
Status --> $git status
Lift Cycle of File Status | ( Untracked -> Unmodified -> Modified -> Staged)
Try to reset --> $git resert HEAD <file>
Remove files --> $rm <file>
Remove files (git) --> $git rm <file>
Remove files (git cache) --> $git rm --cached <file>
Help Command --> $git help <COMMAND>
Move files --> $git MV <NAME> <NEW NAME>

>>>>>>> b629648c82d65c7c502866109d9273a3ee109c11
