# 创建函数部署包

函数部署包是函数代码和依赖项的zip文件，在创建zip文件时，仅包含代码及其依赖项，而不包含文件夹。用户可以通过本地创建函数部署包并上传至function或直接在控制台在线编写代码。


 

**简单场景**-自定义代码依赖库可使用京东云提供的OSS、API网关SDK库，若只有一个代码文件，您可以通过控制台代码编辑器。控制台会将代码及相关的配置信息自动压缩至一个能够运行的部署程序包中。

 
**高级场景**-如果编写的代码需要用到其他资源（如使用Web框架进行Web编程，使用数据库连接库用于执行数据库命令等），则需要先在本地环境创建函数部署程序包，然后再使用控制台上传部署程序包。

 

**打包要求**

Function规定函数部署包的格式必需为.zip格式。打包时，对目录内容进行打包，而非目录本身；打包完成后，入口函数文件需要位于包内的根目录。

* 在Windows下打包时，可以进入函数代码目录，全选所有文件以后，单击鼠标右键，选择“压缩为.zip文件”，生成部署程序包。打开zip包浏览时，包内应该直接包含入口程序与其他库。

* 在Linux下打包时，可以进入函数代码目录，通过调用zip命令将源文件指定为代码目录下的所有文件，生成部署程序包，例如： `zip /codefile/func_code.zip * -r`。