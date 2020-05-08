# Npm

### 镜像地址

**查看**

    npm get registry

**修改**

    npm set registry [url]

### 用户信息

**登录**

    npm login

会依次输入 Username, Password, Email 三个信息

**退出**

    npm logout

### 配置

**查看缓存目录**

    npm config get chache

**修改缓存目录**

    npm config set cache


### 发布 npm 包

**必要条件**

```
package.json
README.md
```

**package.json**

```
{
  "name": "项目名称",
  "version": "版本信息",
  "main": "入口文件",
  "keywords": ["关键词"],
  "description": "描述"，
  "author": "作者",
  "license": "协议"
}
```

**提交**

```
//登录
npm login

// 推送
npm publish --access=public
```
