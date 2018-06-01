# m4sterbunny.github.io

[![dependencies Status](https://david-dm.org/hexojs/hexo/status.svg)](https://david-dm.org/hexojs/hexo)
A fast, simple & powerful blog framework, powered by [Node.js](http://nodejs.org).

## Features

- Update news on the site
- Support for GitHub Flavored Markdown plugins
- One-command deploy to GitHub Pages.

## Quick Start

- Fork repository
- Edit content
- Use run.sh to deploy to GitHub Pages.
- Pullback to repository
![use pull](https://github.com/m4sterbunny/m4sterbunny.github.io/master/ImagesForSiteInstall/use-pull.png "Pull to repo")

## Installation from 0
* Install node.js here https://nodejs.org/en/
* Install git here https://git-scm.com/

``` bash
$ npm install hexo-cli -g
```
**Setup your page**
``` bash
$ hexo init SkillingUp
$ cd SkillingUp
```
**Generate static files**
``` bash
$ hexo generate
//generates files in public folder
```
**Start the server**
- check `_config.yml`
``` php
url: http://localhost/:4000
root: /
```
``` bash
$ hexo server
```
- open browser make sure it works
**Create a new post**
``` bash
$ hexo new "New Page"
```

## Setup to upload to github pages
* Install node.js and git.

``` bash
$ git clone https://github.com/m4sterbunny/m4sterbunny.github.io.git
$ git clone https://github.com/m4sterbunny/SkillingUp.git
```
**Start the server**

Edit `_config.yml`
``` php
url: https://m4sterbunny.github.io
root: /
```
 Install hexo deployer
 ```bash
 npm install hexo-deployer-git --save
 ```
 Add in the end of `_config.yml`
 ``` php
 deploy:
   type: git
   repo: https://github.com/EvilEpicCoder/m4sterbunny.github.io.git
   branch: master
   message: update
 ```
 Now it update your `public` folder to independent repository `m4sterbunny.github.io.git`

 ## Collaboration
 * Install node.js and git.
 * fork two repository
 ![fork repository](https://github.com/m4sterbunny/m4sterbunny.github.io/master/ImagesForSiteInstall/fork.png "fork it")
 * Start working with it
 * use `run.sh` (in windows just click twice) it will update
 ``` bash
 $ https://github.com/NEW_USER/m4sterbunny.github.io.git
 ```
 * Push as - pull request
 ![use pull](https://github.com/m4sterbunny/m4sterbunny.github.io/master/ImagesForSiteInstall/use-pull.png "Pull to repo")
 * admin `m4sterbunny` must review push and make merge or refuse



## More Information

- Visit the [Awesome Hexo](https://github.com/hexojs/awesome-hexo) list
- Read the [documentation](https://hexo.io/)
- Find solutions in [troubleshooting](https://hexo.io/docs/troubleshooting.html)
- Join discussion on [Google Group](https://groups.google.com/group/hexo)
- See the [plugin list](https://hexo.io/plugins/) and the [theme list](https://hexo.io/themes/) on wiki
- Follow [@hexojs](https://twitter.com/hexojs) for latest news
