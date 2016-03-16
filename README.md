# IMC-git101
Generae ssh key ad add to Gtithub
1.use command "$ssh-keygen"
2.copy data in id_rsa.pub
3.setting ssh key on github

Testing SSH connection
use command "$SSh -T git@github.com"

Add remote
use command "$git remote add [NICKNAME] [Remote url]"

Remove remote
use command "$git rm [NICKNAME]"

Rename remote
use command "$git rename [OLD NICKNAME] [NEW NICKNAME]"

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

