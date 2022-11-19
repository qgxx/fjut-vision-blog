# Website

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```


## 如何上传本地文件至doc
1.使用git将项目克隆到本地
```
git clone https://github.com/typical-motion/fjut-vision-blog.git
```

2.在``docs``目录下编写``.md``文件

**Tips:** 如果需要图片，则需要将图片添加到``static``目录下  
在``.md``文件下使用相对路径

3.在本地验证是否有bug  
```npm run start```  

4.上传代码至GitHub  

```  
git config --global http.postBuffer 1048576000
git push -u origin master
```
