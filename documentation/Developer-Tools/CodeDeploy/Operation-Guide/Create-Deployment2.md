## 新建部署

进入到“新建部署”页，有以下选项：

- 部署描述：非必须，为本次部署的描述信息
- 部署来源：支持多种部署来源，包括“URL上传”、“云编译”、“对象存储”。若选择“URL上传”，那么，需填写URL地址及MD5；若选择“云编译”，需选择云编译的项目名称及构建成功的构建序号；若选择"对象存储"，需选择对象存储空间及目录
- 文件类型：选择包类型
- 部署操作命令：您可选择将操作命令打包进代码包中，或由页面填写。

   - 输入部署操作命令：提供了方便易上手的表单方式，可满足多数用户的基本需求，选择“表单”填写功能，填写具体操作命令。同时为应对复杂的操作命令，也可支持yaml文件的填写。书写规范详见“操作指南-AppSpec”
  
      - 部署路径：最多支持5组源和目标，具体详见“操作指南-AppSpec文件中的source和destination”
     
      - 执行账户：即执行部署操作中的hooks时，所使用的账户，此账号需为系统中已有账户，否则将无法部署成功
     
      - 超时时间：各脚本执行的超时时间，单位为秒
     
      - 停止脚本：回滚及更新部署时，所用到的停止程序的脚本
     
      - 启动脚本：回滚及更新部署时，所用到的启动程序的脚本
     
      - 检查脚本：部署完成后，检查部署结果的脚本。返回0为成功，返回非0为失败
     
   - 使用代码根目录的appSpec.yml：在代码根目录中，添加包含了部署操作命令的appSpec文件，文件名为appSpec.yml。书写规范详见“操作指南-AppSpec文件”

![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/operation19.png)


填写部署任务信息后，请点击“部署”，将触发部署操作。
