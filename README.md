
<h1 align="center" style="margin: 30px 0 30px; font-weight: bold;">排课选课系统 v1.0</h1>
<h4 align="center">基于RuoYi+SpringBoot+Vue的排课选课系统</h4>
<p align="center">
	<a href="https://gitee.com/y_project/RuoYi-Vue"><img src="https://img.shields.io/badge/RuoYi-v3.8.8-brightgreen.svg"></a>
	<a href="https://gitee.com/y_project/RuoYi-Vue/blob/master/LICENSE"><img src="https://img.shields.io/github/license/mashape/apistatus.svg"></a>
</p>

## 平台简介

排课选课系统是一套基于若依框架开发的教务管理平台，适用于高校、培训机构的课程安排与选课管理。

* 前端采用Vue、Element UI。
* 后端采用Spring Boot、Spring Security、Redis & Jwt。
* 权限认证使用Jwt，支持多终端认证系统。
* 支持加载动态权限菜单，多方式轻松权限控制。
* 基于若依框架进行二次开发，保留原有功能的同时扩展教学管理功能。

登录账号：
超级管理员：admin/admin123可以查看所有数据以及页面
普通管理员：zzy1/123456  可以查看所有数据以及页面
教师： 林雪/123456      可以查看自己的课程还有自己课程的选课情况，课程改分
学生：zzy/123456



## 内置功能

1.  用户管理：管理教师、学生等系统用户，配置权限和基本信息。
2.  专业管理：配置学校专业信息，支持多级专业结构。
3.  班级管理：配置班级信息，关联专业和年级。
4.  教室管理：管理教学场所，支持各类教室类型。
5.  课程管理：设置课程基本信息，包括学分、课时等。
6.  学期管理：创建和管理学期信息。
7.  排课管理：教师和管理员可进行课程排课，支持不同限制等级：
   - 班级级别：课程仅针对特定班级开放
   - 专业级别：课程针对特定专业的学生开放
   - 年级级别：课程针对特定年级的学生开放
8.  选课管理：学生可在选课时间内进行选课和退课操作。
9.  自动排课：支持根据配置规则自动生成课表。
10. 选课时间：管理员可设置每学期的选课时间段。
11. 选课冲突检测：自动检测并阻止时间冲突的选课。
12. 教师评分：教师可对已修课程进行评分和管理。
13. 课程表视图：学生可以列表或课程表方式查看已选课程。
14. 成绩管理：记录和管理学生的课程成绩。
15. 数据统计：统计选课人数、通过率等数据。

## 系统架构

- 系统基于前后端分离架构，前端使用Vue+ElementUI，后端使用SpringBoot。
- 数据库采用MySQL，支持主流数据库。
- 缓存采用Redis，提高系统响应速度。
- 权限管理采用RBAC模型，灵活配置不同角色权限。

## 主要特色

1. **多级排课限制**：支持按班级、专业、年级三个级别进行排课限制
2. **智能选课处理**：自动检测时间冲突、人数限制等条件
3. **灵活的选课时间配置**：可针对不同学期设置不同的选课时间段
4. **双视图课表**：支持列表视图和课程表视图，满足不同使用习惯
5. **完善的权限控制**：基于角色的精细权限控制，确保数据安全

## 使用角色

- **管理员**：负责系统配置、基础数据维护、用户管理等
- **教师**：进行排课、查看选课学生、录入成绩等
- **学生**：进行选课、查看课表、查询成绩等

## 部署说明

详细部署说明请参考系统文档。默认运行环境要求：
- JDK 1.8+
- MySQL 5.7+
- Redis 5.0+
- Node.js 12+

## 系统截图

管理员：
<img width="956" alt="beed7f9b3031d458b052984e78a6a48" src="https://github.com/user-attachments/assets/c4893d93-fe5b-4da0-87e0-5eabfaf9b38b" />

<img width="956" alt="f0f30f6658d06602058768b6487d4d8" src="https://github.com/user-attachments/assets/6a4ef628-6bf3-46f0-9a26-044ac0ec0114" />

<img width="956" alt="7ee693aee35a2a124a8b9a1aeeb0074" src="https://github.com/user-attachments/assets/6b9a3be1-8036-4f27-9097-c428f03e61d2" />
<img width="956" alt="0eb42fc77cb1ec43d13fb30b0efd04c" src="https://github.com/user-attachments/assets/28077cc9-1587-47d6-936c-2b9f733c0061" />
<img width="956" alt="22e112cac33928025de2714d5e1c4b5" src="https://github.com/user-attachments/assets/e31ed84b-3d57-4a09-8f04-9f8cea8afa91" />
<img width="956" alt="f75ee2eab000cec34982f742b07f98f" src="https://github.com/user-attachments/assets/260fed9b-9049-4bfa-b453-8ba5de662eb8" />

<img width="956" alt="330a6a3f0ccf4f49dd4063e158507bb" src="https://github.com/user-attachments/assets/448e256b-11bc-4bc8-b3a2-93a5e866e13a" />
<img width="956" alt="6561b0dfa54d7591a9890a7d81c0951" src="https://github.com/user-attachments/assets/189db8b3-5c9c-4e09-b01f-5a434decabfc" />
<img width="956" alt="93ac36eb80e9fe69f858880203f59e8" src="https://github.com/user-attachments/assets/15ad3a8b-5949-4b2a-8096-891634991c02" />
<img width="956" alt="1aee1e2d44c1aa5cc3280f490aabac3" src="https://github.com/user-attachments/assets/67e7b0ec-b461-4aec-808e-41abbf9c09f5" />
<img width="1074" alt="2f58035fd1c46dc551aa0a469616674" src="https://github.com/user-attachments/assets/1a5befcf-679f-4166-8515-f6a62d28f2d1" />


教师：
<img width="1074" alt="1fdaaacd0722ea4c562c2645e459b7d" src="https://github.com/user-attachments/assets/9f244277-c859-4bc1-8b70-209c79da3fb5" />
<img width="1074" alt="e0fdaa463f1e631813a33420459b66b" src="https://github.com/user-attachments/assets/cb196f9b-321c-40ec-a90e-58cdf85ab697" />


学生：
<img width="1080" alt="3f62ec50b53fb657d96eb1d15afb3f0" src="https://github.com/user-attachments/assets/e2a2ef48-f06d-4265-896f-1c5a0b3bb255" />

<img width="1080" alt="8365daf85f60b35a9f2baefabc02dd8" src="https://github.com/user-attachments/assets/6960eddf-2518-41a6-baf0-7d6abc713408" />

<img width="1080" alt="2d5005d336f7052d1a1ed3450c77d9f" src="https://github.com/user-attachments/assets/e9c259ea-39ab-499f-9ee4-fc7bf857fc5c" />


## 联系方式

如有问题请联系 微信 
<img width="1080" alt="2d5005d336f7052d1a1ed3450c77d9f" src="https://github.com/user-attachments/assets/194a4d04-675a-4b8c-af7a-f504fbda4464" />

