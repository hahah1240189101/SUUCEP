## README

校园组队与竞赛信息服务平台

广州交通大学-2023届软件工程192-毕业设计

联系方式：13168162412（微信）

实现了：

1. 较为精美的UI
2. 各类实体数据的分页展示以及其详情页展示
3. 学生、教师、管理员对个人信息、竞赛、活动、队伍、帖子、公告、新闻等实体的增删改查
4. 不同角色对应不同权限
5. 各类实体中所需的文件的上传与下载
6. 定时任务控制竞赛、活动的实时进程
7. 定时任务计算展示数据（优秀个人、竞赛排行榜、队伍星级等）
8. 简单的token登录认证与鉴权
9. 同一账号多端登录踢下线、管理员封禁账号踢下线
10. 帖子二级评论
11. 简易的消息推送，推送类消息使用socket.io，其余消息做持久化



技术栈：

1. 前端：Vue2.0 + ElementUI + moment + mavon-editor
2. 登录：Security + BCrypt + Jwt + Redis + Socket.io
3. 服务：vuex + axios + SpringBoot + Mybatis-Plus + MySql



食用方式：

1. D盘新建文件夹Project，将项目移动到此文件夹内。
2. 项目中有两个子文件夹，_ui后缀为vue2.0项目，另一个是springboot项目。
3. springboot项目中graduation_project_db.sql为mysql数据库文件。
4. idea打开springboot项目，配置maven仓库路径，修改application.yml中mysql密码。
5. 启动redis，不需配置。
6. 启动springboot项目，运行CampusTeamContestInformationServicePlatformApplication。
7. 启动前端项目，vscode打开_ui后缀项目，新建终端输入npm run serve。
8. 浏览器打开http://localhost:8080/。



项目图：



登录

![2.登录](D:\Project\校园组队与竞赛信息服务平台\项目截图\2.登录.png)



注册

![3.注册](D:\Project\校园组队与竞赛信息服务平台\项目截图\3.注册.png)



首页

![4.首页](D:\Project\校园组队与竞赛信息服务平台\项目截图\4.首页.png)



竞赛大厅

![5.竞赛大厅](D:\Project\校园组队与竞赛信息服务平台\项目截图\5.竞赛大厅.png)



活动大厅

![6.活动大厅](D:\Project\校园组队与竞赛信息服务平台\项目截图\6.活动大厅.png)



组队大厅

![7.组队大厅](D:\Project\校园组队与竞赛信息服务平台\项目截图\7.组队大厅.png)



茶话会

![8.茶话会(小型论坛)](D:\Project\校园组队与竞赛信息服务平台\项目截图\8.茶话会(小型论坛).png)



竞赛详情页

![9.竞赛详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\9.竞赛详情页.png)

![9.竞赛详情页2](D:\Project\校园组队与竞赛信息服务平台\项目截图\9.竞赛详情页2.png)



活动详情页

![10.活动详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\10.活动详情页.png)



队伍详情页

![11.队伍详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\11.队伍详情页.png)



个人详情页

![12.个人详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\12.个人详情页.png)帖子详情页

![13.帖子详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\13.帖子详情页.png)



帖子评论

![14.帖子评论](D:\Project\校园组队与竞赛信息服务平台\项目截图\14.帖子评论.png)



消息盒子

![15.消息盒子](D:\Project\校园组队与竞赛信息服务平台\项目截图\15.消息盒子.png)



导航卡片

![16.导航卡片](D:\Project\校园组队与竞赛信息服务平台\项目截图\16.导航卡片.png)



个人信息编辑

![17.个人信息编辑](D:\Project\校园组队与竞赛信息服务平台\项目截图\17.个人信息编辑.png)

![17.个人信息编辑2](D:\Project\校园组队与竞赛信息服务平台\项目截图\17.个人信息编辑2.png)



我的竞赛

![18.我的竞赛](D:\Project\校园组队与竞赛信息服务平台\项目截图\18.我的竞赛.png)



发布竞赛

![19.发布竞赛](D:\Project\校园组队与竞赛信息服务平台\项目截图\19.发布竞赛.png)



竞赛管理

![20.竞赛管理](D:\Project\校园组队与竞赛信息服务平台\项目截图\20.竞赛管理.png)



我的活动

![21.我的活动](D:\Project\校园组队与竞赛信息服务平台\项目截图\21.我的活动.png)



发布活动

![22.发布活动](D:\Project\校园组队与竞赛信息服务平台\项目截图\22.发布活动.png)



我加入的队伍

![23.我加入的队伍](D:\Project\校园组队与竞赛信息服务平台\项目截图\23.我加入的队伍.png)



我创建的队伍

![24.我创建的队伍](D:\Project\校园组队与竞赛信息服务平台\项目截图\24.我创建的队伍.png)



创建队伍

![25.创建队伍](D:\Project\校园组队与竞赛信息服务平台\项目截图\25.创建队伍.png)



我的帖子

![26.我的帖子](D:\Project\校园组队与竞赛信息服务平台\项目截图\26.我的帖子.png)



写帖子

![27.写帖子](D:\Project\校园组队与竞赛信息服务平台\项目截图\27.写帖子.png)



公告或新闻详情页

![28.公告或新闻详情页](D:\Project\校园组队与竞赛信息服务平台\项目截图\28.公告或新闻详情页.png)



平台管理&公告新闻管理

![29.平台管理&公告新闻管理](D:\Project\校园组队与竞赛信息服务平台\项目截图\29.平台管理&公告新闻管理.png)

![29.平台管理&公告新闻管理2](D:\Project\校园组队与竞赛信息服务平台\项目截图\29.平台管理&公告新闻管理2.png)


add dev test