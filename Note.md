### add 命令
`git add -u`, 只会添加已经track的文件, 不会添加未track的文件

### 连接远程仓库
1. 首先在远端建立一个仓库
2. 然后在本地建立一个仓库
3. 连接本地仓库和远程仓库
    ```bash
    git remote add origin https://github.com/NoahF112/GitLearning.git
    ```
    <br> origin 是远程仓库的名字, 可以自己定义. 命令的意思是, 给远程仓库起了一个名字叫做 origin, 并且将远程仓库的地址设置为URL, 并在最后加上.git, 表示这是一个git仓库

4. 将本地仓库的内容推送到远程仓库
    ```bash
    git push -u origin master:master
    ```
    <br> -u 表示将本地仓库和远程仓库关联起来, 以后就可以直接使用`git push`命令推送本地仓库的内容到远程仓库了
