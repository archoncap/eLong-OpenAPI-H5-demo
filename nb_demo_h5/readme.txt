当前版本：branch1.0.0
2016年12月15日
****************************** 配置说明 **************************************
第一步：修改配置文件:
/nb_demo_h5/src/main/resources/conf/custom/env/common.properties

第二步：maven命令打包
clean install -Dmaven.test.skip=true

第三步:发布到web容器上，打开首页

第四步：IP白名单配置
打开首页时，Console窗口会提示要配置的IP，找elong工作人员后台配置IP白名单
****************************** 配置说明 **************************************


****************************** 项目结构 ************************************
1.项目架构：Spring MVC + JSP + AUI + jQuery
2.后端结构说明：
	controller:负责基本的参数验证以及业务逻辑层service的调用；
	service：负责主要业务逻辑的封装任务；调用rpc层；
	rpc: 封装了所有elongAPI的调用过程，每个API接口对应着一个Api类；
	model：供所有层调用，包含了所有用到的JavaBean；
	util: 工具类集中包
****************************** 项目结构 *************************************


****************************** 其他说明 **************************************
1.项目前端页面制作比较粗略，该项目只做演示作用，代理商可以根据自身公司的产品要求展示元素；
2.为了起到演示作用，该项目的订单并未持久化。代理商在具体开发工程中需根据业务需要进行持久化；
3.该项目的下订单过程，并未引进用户的概念。
4.该项目的下订单过程分为两步：1）创建订单；2）支付订单；
5.该项目为示例demo项目，仅供参考；
****************************** 其他说明 **************************************
