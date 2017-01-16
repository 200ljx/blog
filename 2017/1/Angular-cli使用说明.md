#  开发日记

---

## 一、安装环境依赖

### node 6.9.2/npm 3.10.9
### 检查版本` node -v  `` npm -v `
[下载地址 https://nodejs.org/en/](https://nodejs.org/en/)

---

### git
### 检查版本 `git --version`
[下载地址 https://git-scm.com/downloads](https://git-scm.com/downloads)

---

# 二、构建

### 全局安装angular-cli
### `npm install -g angular-cli`

### 执行ng命令 启动项目

### `ng new PROJECT_NAME`
### `cd PROJECT_NAME`
### `ng serve`

### 参考链接
### [https://github.com/angular/angular-cli](https://github.com/angular/angular-cli)
### [https://cli.angular.io/](https://cli.angular.io/)

---

# 三、angular2学习
### 参考资料
### [http://origin.angular.live/docs/ts/latest/quickstart.html](http://origin.angular.live/docs/ts/latest/quickstart.html)

---

# 四、问题收集
### 1、单页面应用apache链接刷新404解决办法？
 根目录添加文件.htaccess 并修改如下节点

    <IfModule mod_rewrite.c>
        RewriteEngine On
        RewriteCond %{REQUEST_FILENAME} !-f
        RewriteCond %{REQUEST_FILENAME} !-d
        RewriteCond %{REQUEST_URI} !index
        RewriteRule (.*) index.html [L]
     </IfModule>
