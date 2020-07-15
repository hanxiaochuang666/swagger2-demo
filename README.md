## swagger2自动生成离线html和PDF文档
使用方式：
* 可以参考我的博客：https://blog.csdn.net/han_chuang/article/details/98748944
* 下载后导入到idea中，然后等待pom下载相关依赖
* 下载完依赖后，在target.swagger下面的swagger.json文件中，把内容替换成你自己的项目对应的swagger在线文档的json文件地址(比如：http://localhost:8088/v2/api-docs)
* 然后使用maven工具栏点击clean和test就会在target.asciidoc.html和target.asciidoc.pdf生成对应的文档信息

## 生成pdf
由于原生的生成pdf有问题，中文显示不全或者乱码，所以需要改变默认字体，所以直接使用**项目中的**
asciidoctorj-pdf-1.5.0-alpha-zh.16.jar包替换掉本地仓库的就行了，注意名字要改成原生jar包的名字

