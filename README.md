# IMC-git101
<h1>install git</h1>
เร่ิมจาก dowload   file  http://git-scm.com </br>
หลังจาก install เรียบร้อยแล้ว  </br>
<h1>เริ่มทำงานโดยใช้คำสั่ง</h1>
$git config --gobal user.name "your name" -- > ระบุชื่อที่เราต้องการ </br>
$git config --gobal user.email "your email" --> ระบุชื่อ Email ที่เราต้องการ </br>
$git config -l --> เพื่ดูว่ารายการที่เราเพิ่มทั้ง 2 รายการนั้นได้เพิ่มเรียบร้อยหรือไม่ </br>
<h1>Creare a repository</h1>
select git bash --os window </br>
open Terminial --os mac/linux </br>
<h1>เริ่มเข้าใช้งาน git </h1>
เข้าไปหน้า git bash เพื่อจะเข้าสู่การป้อนคำสั่เริ่มจาก ส้ราง folde </br>r 
$mkdir workspace -- > workspec = ชื่อสามารถกำหนดตามความต้องการ  </br>
$git init set directory นั้้นให้ git รู้จัก </br>
pwd  --> คำสั่งแสดง Current Path</br>

﻿$git status คือ คำสั่งดูstatusของปัจจุบัน  </br>
$git touch ตามด้วยชื่อFile คือ คำสั่งสร้างFile </br>
$git add ตามด้วยชื่อไฟล์  คือ คำสั่งaddเข้า stage (การเก็บเข้าStage คล้ายกับการสร้าง Temp File ก่อนการ Commit)  </br>
$git add . คือ คำสั่งadd Fileที่มีอยู่ทั้งหมดเข้า stage </br>

<h1>Ignore files and folders</h1>
- ไฟล์ หรือโฟลเดอร์ที่มีนามสกุล .gitignore จะไม่ถูก git สนใจก่อนที่จะทำการ commit

<h1>View staged and unstage change</h1>
- เมื่อเราพิมพ์คำสั่ง $git status แล้ว git จะทำการแสดงสถานะของ branch ในขณะนั้นเช่น แสดงไฟล์ที่เพิ่มเข้ามาใหม่, ไฟล์ที่มีการเปลี่ยนแปลง, ไฟล์ที่มีการลบ เป็นต้น
- เป็นประโยชน์ในการตรวจเช็คว่าหลงลืมอะไรหรือเปล่า ก่อนที่จะทำการ commit โค้ดขึ้นไป

<h1>See difference of files</h1>
- ใช้คำสั่ง diff เพื่อใช้เปรียบเทียบความแตกต่าง สามารถระบุได้ทั้งในระดับไฟล์ หรือในระดับ commit ได้
- หากต้องการเปรียบเทียบความแตกต่างระหว่างโค้ดของเรา กับ commit ล่าสุด

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

