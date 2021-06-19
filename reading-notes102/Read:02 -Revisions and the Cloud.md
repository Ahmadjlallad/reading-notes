##### - from : Ahmad Jallad.
##### - to   : Emad (my friend wich he doesn't know anythaing about terminal ).

Hi Emad hope you will, here some useful Remote Repositories command if you intrested.

#### Remote Repositories: 
In collaboration work or team work space to make working in new project easier Remote Repositories is a must so here is some uesfull comand that use git, **Git:** is a DVCS that stores data in a file system made up of snapshots.

- useing git you can Cloned Seeing and Adding data and much more to your server.

- first ```git remote``` show you short names of the files in the Repositories but you can use ```git remote -v``` to view URLs and shot name.

- to add files smplie use ```git remote add "shortname follwed by URL"```
- Fetching help you grab data you did't have from a remote project ```git fetch [remote-repo name]```so if you did't pulled to your repo since last time you cloned ```git fetch [remote-repo name]``` can solve the problem.

- when you finsh working on your files you should uploud it for your teammates here is your convenient command ```git push [remote repo name] [local branch name on your hard drive]```
- For example you need to push file called Ahmad in your local hard drive folder jallad first navigate to the folder using ```cd jallad```
which means change directory to jallad then up loud it to your serever black clover```git push [black clover] [jallad]``` but only if you have write access for the server and if your team mates haven't pushed yet meaing that if any of your team mate pushed anything you have to pull it before pushing
- lastly to remove or rename anything 
  - use```$ git remote rm Ahmad``` (```rm``` = Remove file)
  - to Rename use ```$ git remote rename Ahmad Ahmadjallad```
- you can use ```$ git remote``` to cheack files to stat after the changes as stated above.

As always I hope you learned something 

your sincerely _Ahmadjallad_
