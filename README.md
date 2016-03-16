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
เข้าไปหน้า git bash เพื่อจะเข้าสู่การป้อนคำสั่เริ่มจาก ส้ราง folde </br>
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
use command "$ssh -T git@github.com" <br/>

<h1>Add remote</h1>
use command "$git remote add [NICKNAME] [Remote url]" <br/>

<h1>Remove remote</h1>
use command "$git remote rm [NICKNAME]" <br/>

<h1>Rename remote</h1>
use command "$git remote rename [OLD NICKNAME] [NEW NICKNAME]" <br/>

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

<h1>Remote Repository*******<h1>

1) git push => copy source code from Local to Remote Repository
    push to remote => used syntax "git push [NICKNAME] [BRANCH]"
    Fetch and Merge => use syntax "git pull [NICKNAME] [BRANCH]"<br/>
2) git clone => combine "git init" + "git remote" + "git pull"<br>
3) git pull => pull source code from Remote Repository to Local
    "git pull" make sequence as fetch then merge<br/>
    => git fetch [NICKNAME] only pull source code, not auto merge<br/>
    => git merge [BRANCH]<br/>
	=> git rebase [BRANCH]<br/> 

<br/>
Commit --> $commit -m "Your Messsage"<br/>
Status --> $git status<br/>
Lift Cycle of File Status | ( Untracked -> Unmodified -> Modified -> Staged)<br/>
Try to reset --> $git resert HEAD <file><br/>
Remove files --> $rm <file><br/>
Remove files (git) --> $git rm <file><br/>
Remove files (git cache) --> $git rm --cached <file><br/>
Help Command --> $git help <COMMAND><br/>
Move files --> $git MV <NAME> <NEW NAME><br/>
<br/>

<img src="https://fbcdn-sphotos-e-a.akamaihd.net/hphotos-ak-xta1/v/t1.0-9/12106758_616016458545698_2281685477610694246_n.jpg?oh=397b045e98cb10671e962b84bacca812&oe=57577EAB&__gda__=1468672034_b063312705848bfcbd624b3c6a0ab18d"/>