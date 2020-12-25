# git

![05](readme_image/05.png)

| git仓库          | 暂存区             | 工作目录            |
| ---------------- | ------------------ | ------------------- |
| 用于存放提交记录 | 临时存放被修改文件 | 被Git管理的项目目录 |

## git配置

```shell
# 配置提交人姓名
git config --global user.name 提交人姓名
git config --global user.name myqz

# 配置提交人邮箱
git config --global user.email 提交人邮箱 
git config --global user.email ambition292@163.com

# 查看git配置信息
git config --list
```

## git提交

```shell
# 初始化git仓库
git init

# 查看文件状态
git status 

# 追踪文件,提交到暂存区
git add 文件列表
git add readme.md

# 向仓库中提交代码
git commit -m 提交信息  
git commit -m 添加readme

# 查看提交记录
git log` 
```

## git撤销

 ```shell
# 用暂存区文件 >>覆盖>> 工作目录文件
git checkout 文件
  
# 将文件从暂存区中删除
# 工作目录中文件还存在
git rm --cached 文件

# 将git仓库中指定的更新记录恢复出来，并且覆盖暂存区和工作目录
# 版本回退 git log 查看commitID -> 注意版本从高到低
git rest --hard commitID
 ```

  