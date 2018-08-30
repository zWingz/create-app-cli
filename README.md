# create-app cli
    根据vueCli改写,减少部分功能.
    只留下初始化部分
    可以从gitlab/github/本地文件中的项目模板构建新应用

## 使用方法

### 安装
```bash
    npm i @zzwing/create-app -g
```

### 使用
```bash
    create-app init <template-name> <project-name> [-c]
```
如果需要通过git clone来拉取项目.请使用`-c` 参数


### 本地文件
你可以使用本地模板作为你的新项目模板

``` bash
    create-app init ~/fs/path/to-custom-template my-project
```

#### 通过其他仓库获取
The short hand repository string to download the repository from:

- GitHub - `github:owner/name` or simply `owner/name`
- GitLab - `gitlab:owner/name`
- Bitbucket - `bitbucket:owner/name`


## Examples
Using http download from Github repository at master.
```bash
create-app init path/to/repo myProject
```

Using git clone from Bitbucket repository at my-branch.
```bash
create-app init bitbucket:path/to/repo#my-branch myProject
```

Using http download from GitLab repository with custom origin.
```bash
create-app init gitlab:mygitlab.com:path/to/repo#my-branch myProject
```

### 路径具体写法请参考
[download-git-repo](https://github.com/flipxfx/download-git-repo/blob/master/README.md)
