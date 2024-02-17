 <center>
     <h1>田金荣</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
             173333401931
         </span>
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             1819324794@qq.com
         </span>
     </div>
 </center>

 ## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息 

 - 男,2000年出生
 - 求职意向：Java后端开发
 - 工作经验：1.5年
 - 期望薪资：15k

## <img src="assets/graduation-cap-solid.svg" width="30px"> 教育经历

- 本科,河北地质大学,网络工程专业,2018.9~2022.7
- 通过CET4/6英语等级考试,PAT甲级满分

## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

- 杭州迅杭有限公司,指标组,Java开发工程师,2022.7~2023.12,负责指标设计开发、资产树设计开发等

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历
<h3>项目名称：FILIB+指标库/指标集市</h3>
- 项目简介：FILIB是指标框架,主要用于指标的计算;指标库/指标集市为前台展示项目,主要用于获取FILIB的计算结果并进行组装展示;指标集市对指标库的方案组装进行了重构,对新客户推荐指标集市,老客户仍使用指标库
- 项目技术：使用SpringBoot;支持Eureka和Nacos注册中心;支持Mysql/Oracle/StarRocks等数据库;支持使用Redis缓存;

主要实现：
1. 在FILIB中,完成指标的开发计算工作,比如开发期初组合市值占总净值比等指标或开发基本面对冲归因;优化指标效率,排查现场指标问题,通过Excel验算指标等;
2. 在指标库中,新增接口或调整旧接口支持新的需求;进行接口的效率优化;调整指标库参数,优化落地效率等;
3. 在指标集市中,对指标库代码迁移调整,适配指标集市;开发集市配置等功能,进去前后端联调;指标集市支持SQL指标,使用EasyExcel开发导入导出功能;指标集市支持多数据源,目前仅支持Mysql、Oracle、StarRocks数据源,实现自动建表,字段的自动增减,简化建立落地方案流程;

项目难点：
1. 在FILIB中,开发基本面对冲归因,依据Excel底稿进行调整;优化指标取数和依赖逻辑,提高指标计算效率;
2. 在指标库中,优化资产树落地接口,接口效率由原来的半小时提升至五分钟;排查由于序列化失败,导致方案落地数据不一致问题; 
3. 在指标集市中,支持StarRocks数据库,StarRocks数据库的建表删表规则同Mysql/Oracle相差较大,调整了建表删表规则;

<h3>项目名称：XASC+筛选服务</h3>
- 项目简介：筛选服务主要为切分指标,比如划分股票、基金,则由筛选服务进行切分;XASC为前台展示项目,主要用于配置资产树;
- 项目技术：支持SpringBoot/SpringCloud;支持Eureka和Nacos注册中心;支持Mysql/Oracle等数据库;支持使用Redis缓存;

主要实现：
1. 在筛选服务中,主要完成对筛选指标的开发,修复服务BUG,配置对应的资产属性等;
2. 在XASC中,通过产品文档配置对应资产树,调整资产树界面拖动逻辑等;

项目难点：
1. 在筛选服务中,出现过多线程情况下,使用缓存取数为空的问题;在筛选服务中,如果请求报错,会导致请求上下文未释放,导致下一个请求上下文不生效;
2. 优化资产树刷新大数据规则,修改为异步刷新;优化前端资产树规则自动刷新逻辑,由原来的30秒提升至5秒;

<h3>项目名称：牛客网讨论区 </h3>
- 项目技术：后端采用SpringBoot;前端使用Thymeleaf;采用Mysql、Redis数据库;Kafka消息队列,Elasticsearch搜素引擎;

主要实现：
1. 完成权限,注册,登录,退出,授权功能,使用Redis;使用Spring Mail完成激活邮件和找回密码邮件的发送;使用Kaptcha完成验证码的动态生成
2. 完成首页、站子、评论、私信、日志功能,对发布的评论使用前缀树,进行敏感词过滤;使用@ControllerAdvice和@ExceptionHandle进行统一异常处理;使用注解对事务进行统一管理;使用aop增加日志功能
3. 完成点赞、关注、系统通知功能,使用redis储存点赞,关注高频功能数据;使用Kafka推送系统通知;使用Elasticsearch完成关键字搜索功能,对符合词进行高亮显示。
4. 实现热度排行,使用SpringQuartz进行分布式任务定时刷新,使用Redis进行缓存,提高效率,使用ElasticSearch进行搜索
5. 实现网站数据统计,使用Redis的HyperLogLog,统计独立访客;使用Redis的Bitmap统计日活跃用户;

项目难点：
1. 热度排行刷新功能;首先是热度分数的计算,越新的姑子分数应该越高
2. 对于点赞数、 评论数、精华分的计算使用log,实现相对平稳的过渡
3. 刷新时间,为5分钟,避免频繁刷新,使用本地缓存,提高查找效率;
4. 引入SpringQuartz进行分布式刷新。

## <img src="assets/tools-solid.svg" width="30px"> 技能清单

- 熟练掌握Java基础,掌握J2EE基本架,了解多线程,集合操作等基础技能 
- 熟悉Maven项目配置管理工具,熟悉常用的项目管理工具git
- 熟悉Spring,Spring MVC,Springboot,Mybatis主流开源框架
- 熟悉MySql、Oracle、Redis等常用数据库,了解StarrRocks数据库、Kafka消息队列
- 了解SpringCloud分布式框架
- 了解Linux系统及常见命令,有Linux下排查项目的实际经验