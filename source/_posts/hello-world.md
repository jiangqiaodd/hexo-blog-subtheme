---
title: How to create a new blog
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Preparation 

### NodeJs
```
refer: https://nodejs.org/en/
```

### Hexo
```
$npm install -g hexo-cli
```

## Quick Start

### hexo-starter
two choose:
- from earlist(test)
```
$hexo init <folder>
```
- from self github(product)
```
$git clone https://github.com/user-name/hexo-blog.git
$npm install             (会根据配置安装 前端相关依赖)
```

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```
#### Deploy to github site
- first you need create a  github repository like 'jiangqiaodd.github.io'
- secone you should config develop on _config.yml
```
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type:   'git'
  repo:   'https://github.com/jiangqiaodd/jiangqiaodd.github.io.git'
  branch: 'main'
```
- third install deploy-github tool
```
npm install hexo-deployer-git --save
```
- last deploy to github
```
hexo clean 
hexo g 
hexo d
```

### Add CNAME if you want use self domain name
```bash
$echo bridgeofdream.xyz > CNAME
$git add ./
$git commit ./
$git push 
```
More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
