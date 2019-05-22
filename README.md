## swagger2自动生成离线html和PDF文档
使用方式：
* 下载后导入到idea中，然后等待pom下载相关依赖
* 下载完依赖后，在target.swagger下面的swagger.json文件中，把内容替换成你自己的项目对应的swagger在线文档的json文件(比如：http://localhost:8088/v2/api-docs)
* 然后使用maven工具栏点击clean和test就会在target.asciidoc.html和target.asciidoc.pdf
