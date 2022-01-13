## 发布
##### 先安装vsce
```
npm install vsce -g
```
 
##### 创建账号
首先访问 `login.live.com/` 登录你的Microsoft账号，没有的先注册一个，然后访问： `aka.ms/SignupAzure…` ，如果你从来没有使用过Azure，那么就要先创建一个Azure DevOps 组织，默认会创建一个以邮箱前缀为名的组织。


##### 进入组织创建令牌

##### 创建一个发布者
发布者是 visualstudio 代码市场的扩展的唯一身份标识。每个插件都需要在 package.json 文件中指定一个 publisher 字段。
你可以通过 visualstudio 插件市场发布者管理页面创建一个新发布者，
然后使用 `vsce login <publisher name>` , 输入刚才的 token，登陆成功。

##### 发布插件
```
vsce publish
```

发布成功后可能需要一两分钟，才可以在 VS Code 中搜索到，可以直接通过 url 访问

[参考 - 掘金](https://juejin.cn/post/7030250953215311908)
[参考 - vscode官网](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
