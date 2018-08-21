####Git多人协作的工作模式
1.首先可以试图用```rgit push origin <branch-name>```推送自己的修改；
2.如果推送失败，则因为远程分支比你的本地更新，首先要使用```git pull```试图合并；
3.如果合并有冲突,则解决冲突,并在本地提交;
4.如果没有冲突或解决掉冲突后,再使用```git push origin <branch-name>```推送就能成功!
如果```git pull```提示```no tracking information```,则说明本地分支和远程分支的链接关系没有创建，用命令```git branch --set-upsstream-to <branch-name> origin</branch-name>```.
####小结
*查看远程库信息,使用```git remote -v```;
