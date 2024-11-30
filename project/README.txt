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