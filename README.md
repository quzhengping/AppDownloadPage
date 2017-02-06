# 10分钟完成App下载页面编写

差不多前端工作上一段时间完成这样的页面没什么难度。当时项目经理说App发布会在中午2点开始，12点半告诉我要完成这个页面，要求如下：

* 解决手机端兼容性的问题，尤其是小米浏览器
* 解决响应式的问题，iphone5上能显示全
* 在微信中显示提示“在手机浏览器中打开”
* 图片上传到CDN，区域资源全部打包到一个html中并压缩(最终交付一个html)

看样子要上一个Gulp工程了，于是着急的写了一个gulpfile.js，然后吭哧吭哧了差不多1个多小时完成了页面。页面完成后，觉得这样的需求应该不是突发的，日后App发布时的H5下载页都需要写一份，所以将项目当做种子文件，发布到Github上便于以后应对。


## 项目地址 

[点这里]()

## 如何开始

1. 点击上面的地址下载该项目
2. 进入目录运行```npm install```
3. 执行```gulp serve```开始编码

 

## Gulp任务 

| 任务名称  | 任务介绍  |
|:------------- |:-----------------------------:| 
| serve                 | 开启服务，页面修改能自动刷新           | 
| default               | 清理dist目录，执行build                    | 
| build                  | 生成最终文件                                   |  
| serve:dist           | 生成最终文件，并进行预览                 |  
