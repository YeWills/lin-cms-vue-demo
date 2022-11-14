

## 快速上手

### 项目基于 node 12.x 
 项目基于 node 12.x ,否则sass编译报错，
如果是 node 12.x 版本，下面步骤即可打开：

```sh
# clone the project
git clone https://github.com/TaleLin/lin-cms-vue.git

# install dependency
npm install or yarn

# develop
npm run serve or yarn (run) serve
```



### 如果是 node 14.x 版本，可以这样做：
先将node 迁移至 node 12.x，
执行下面命令，让 node-sass 跑完 preinstall 的脚本。
```sh
yarn
```
然后切换到 node 14.x，

```sh
# develop
npm run serve or yarn (run) serve
```
此时会报错，告知要node 12.x 版本，然后推荐你 ` npm rebuild node-sass` ，
执行
```s
 npm rebuild node-sass
 npm run serve 
```
即可正常访问。


## FAQ

### 跨域
通过设置如下文件：
```
//lin-cms-vue-demo/.env.development
VUE_APP_BASE_URL = 'http://localhost:5000/'
```

