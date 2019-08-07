## swagger2自动生成离线html和PDF文档
使用方式：
* 下载后导入到idea中，然后等待pom下载相关依赖
* 下载完依赖后，在target.swagger下面的swagger.json文件中，把内容替换成你自己的项目对应的swagger在线文档的json文件(比如：http://localhost:8088/v2/api-docs)
* 然后使用maven工具栏点击clean和test就会在target.asciidoc.html和target.asciidoc.pdf

## 生成pdf
由于原生的生成pdf有问题，中文显示不全或者乱码，所以需要改变默认字体，所以直接使用项目中的
asciidoctorj-pdf-1.5.0-alpha-zh.16.jar包替换掉本地仓库的就行了
在pom.xml中加入 <dependency> <groupId>org.asciidoctor</groupId> <artifactId>asciidoctorj-pdf</artifactId> <version>1 .5.0-alpha-zh.16</version> </dependency> 
attributes项加入<pdf-style>cn</pdf-style> 其它配置请自行在网上搜索asciidoctorj-pdf配置 