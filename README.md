<h1 align="center">{项目名称}</h1>
<p align="center">
    <a href="https://laravel.com/"><img src="https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel"></a>
    <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D" alt="Vue.js"></a>
    <a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"></a>
    <br>
    <a href="https://ubuntu.com/"><img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu"></a>
    <a href="https://www.nginx.com/"><img src="https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx"></a>
    <a href="https://www.mysql.com/"><img src="https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"></a>
    <a href="https://www.php.net/"><img src="https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white" alt="PHP"></a>
    <a href="https://www.npmjs.com/"><img src="https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white" alt="NPM"></a>
    <a href="https://bun.sh/"><img src="https://img.shields.io/badge/Bun-%23000000.svg?style=for-the-badge&logo=bun&logoColor=white" alt="Bun"></a>
    <br>
    <a href="https://www.jetbrains.com/phpstorm/"><img src="https://img.shields.io/badge/phpstorm-143?style=for-the-badge&logo=phpstorm&logoColor=black&color=black&labelColor=darkorchid" alt="PhpStorm"></a>
    <a href="https://www.postman.com/"><img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman"></a>
    <a href="https://github.com/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
</p>

## ⚙️ 项目初始化

```text
[~/Herd]$ laravel new {项目名称} --pest

 ┌ Would you like to install a starter kit? ────────────────────┐
 │ Laravel Breeze                                               │
 └──────────────────────────────────────────────────────────────┘
 
 ┌ Which Breeze stack would you like to install? ───────────────┐
 │ Vue with Inertia                                             │
 └──────────────────────────────────────────────────────────────┘
 
 ┌ Would you like any optional features? ───────────────────────┐
 │ None                                                         │
 └──────────────────────────────────────────────────────────────┘
 
 ┌ Would you like to initialize a Git repository? ──────────────┐
 │ No                                                           │
 └──────────────────────────────────────────────────────────────┘
 
 ┌ Which database will your application use? ───────────────────┐
 │ MySQL                                                        │
 └──────────────────────────────────────────────────────────────┘
```

```mysql
CREATE DATABASE `{项目名称}` DEFAULT CHARACTER SET `utf8mb4` COLLATE `utf8mb4_general_ci`;
```

```shell
# 运行 Pest 测试代码
./vendor/bin/pest
# 运行 Pint 格式化代码
./vendor/bin/pint
```

## 📝 项目约定和代码规范

### 服务器和版本控制分支

* 开发环境代码库分支：`develop` => `https://{项目名称}.test`
* 测试环境代码库分支：`released` => `https://dev.{项目名称}.com`
* 生产环境代码库分支：`master` => `https://{项目名称}.com`

### Env & Postman 环境配置

* 开发环境接口 host：`https://{项目名称}.test`
* 测试环境接口 host：`https://dev.{项目名称}.com`
* 生产环境接口 host：`https://{项目名称}.com`

### Git 约定式提交规范

#### 提交类型

```text
feat:     新功能
fix:      修复
docs:     文档变更
style:    代码格式(不影响代码运行的变动)
refactor: 重构(既不是增加feature，也不是修复bug)
perf:     性能优化
test:     增加测试
chore:    构建过程或辅助工具的变动
revert:   回退
build:    打包
```

#### 提交格式

```text
<类型>[功能模块(可选)]: <提交概要描述>

[提交正文(可选)]

[脚注(可选)]

-------- 示例 --------

docs(README): 创建项目规范

* 创建项目代码提交约定
* 创建代码格式化规范

issue 666
```
