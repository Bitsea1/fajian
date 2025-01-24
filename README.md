# 学法减分小程序前端源码
## 一、项目简介
本学法减分小程序是基于 Uniapp 框架开发的，旨在帮助用户通过便捷的移动端应用进行学法减分相关知识的学习与练习，以应对交通法规学法减分考试。它充分利用了 Uniapp 跨平台的特性，能够快速编译生成适用于微信小程序、H5 网页等多个平台的应用，为用户提供随时随地学习刷题的便利。

## 二、主要功能
1. **题目浏览**：用户可以按章节或题型分类浏览学法减分的题目，查看题目内容、正确答案以及详细解析，方便系统地学习交通法规知识。
2. **模拟考试**：提供全真模拟考试环境，用户可自定义考试题数、时间限制等参数，在模拟考试过程中，系统自动计时、记录答题情况，并实时显示交卷得分，帮助用户检验学习成果，提前适应考试节奏。
3. **错题整理**：自动收集用户在练习和模拟考试过程中答错的题目，形成错题集。用户可以随时回顾错题，查看正确答案和解析，进行针对性复习，强化薄弱环节，提高学习效率。
4. **学习进度记录**：跟踪并记录用户的学习进度，包括已完成的题目数量、学习时长等信息，用户可在个人中心查看学习统计图表，直观了解自身的学习情况，合理规划后续学习计划。

## 三、技术选型
1. **开发框架**：Uniapp，一款使用 Vue 语法编写应用的框架，能够实现一次开发，多端运行（如微信小程序、H5、Android、iOS 等），大大提升开发效率，减少维护成本。
2. **编程语言**：JavaScript 作为主要的编程语言，用于实现页面交互逻辑、数据处理等功能，结合 Vue.js 的数据绑定和组件化开发模式，使代码结构清晰、易于维护和扩展。
3. **样式处理**：采用 CSS3 和 Less 预处理器来编写样式代码，CSS3 提供了丰富的样式特性，如动画效果、弹性布局等，增强了应用的视觉效果和用户体验；Less 预处理器则允许使用变量、嵌套规则等特性，提高了样式代码的复用性和可读性。

## 四、项目结构说明
```
- src
  - components
    - Home.vue        // 首页组件，包含轮播图、入口菜单等
    - QuestionList.vue // 题目列表组件，展示题目信息
    - QuestionDetail.vue // 题目详情组件，展示单题内容及解析
    - ExamPaper.vue   // 模拟考试试卷组件
    - UserCenter.vue  // 个人中心组件，包含学习进度、错题集等
  - pages
    - index
      - index.js     // 首页页面逻辑文件
      - index.json   // 页面配置文件
      - index.wxml   // 页面结构文件
      - index.wxss   // 页面样式文件
    - question
      - question.js 
      - question.json
      - question.wxml
      - question.wxss
    - exam
      - exam.js 
      - exam.json
      - exam.wxml
      - exam.wxss
    - user
      - user.js 
      - user.json
      - user.wxml
      - user.wxss
  - static
    - images         // 存放图片资源，如 logo、背景图等
    - icons          // 存放图标资源
  - utils           // 工具类文件夹，包含一些通用的方法和函数，如请求封装、数据处理等
  - main.js         // 小程序入口文件，配置全局样式、引入依赖等
  - app.json        // 小程序全局配置文件，配置页面路径、导航栏样式等
  - app.wxss        // 全局样式表文件
```

## 五、使用教程
1. **安装依赖**：确保已安装 Node.js 和 npm，然后在项目根目录下执行 `npm install` 命令，安装项目所需的依赖包。
2. **开发环境搭建**：推荐使用 HbuilderX 或 Visual Studio Code 作为开发工具。创建项目后，将代码克隆到本地开发环境，并在开发工具中打开项目文件夹。
3. **编译运行**：对于微信小程序平台，在 HbuilderX 中点击运行按钮，选择微信小程序模拟器或真机调试；在 VSCode 中，可通过安装微信小程序开发插件，并在终端中使用相关命令进行编译预览。其他平台有相应的编译和运行方式，可根据需求进行配置。

4. **功能测试**：在开发过程中，利用单元测试框架（如 Jest）对各个模块和功能进行测试，确保代码的正确性和稳定性。同时，在真机或模拟器上进行全面的功能测试，检查界面显示是否正常、交互逻辑是否顺畅、数据存储是否正确等。


## 六、前端截图
![微信图片_20250110114540](https://github.com/user-attachments/assets/6cd9069e-0ed1-4292-ae8f-5aa16e994894)
![微信图片_20250110114554](https://github.com/user-attachments/assets/af89262b-60b9-42e8-8c4b-d7be0384140a)
![微信图片_20250110114549](https://github.com/user-attachments/assets/9bc5275c-d79b-41d7-8c05-744eaf58488c)
![5c83d0d01135405299bcc935be876dd](https://github.com/user-attachments/assets/52d9e0a8-7e40-43df-b96f-85d08862d829)

## 七、贡献指南
我们欢迎广大开发者参与到本项目的贡献中来！如果您有任何问题、建议或发现任何漏洞，请按照以下方式向我们反馈：
1. **提交 Issue**：在项目仓库的 Issues 板块创建新问题，详细描述您遇到的问题或提出的建议，尽可能提供详细的复现步骤、错误截图等信息，以便我们更好地理解和解决问题。
2. **提交 Pull Request**：如果您有解决问题的代码或新功能的实现代码，可以在自己的分支上进行修改后，提交 Pull Request。请确保代码符合项目的编码规范和风格要求，并包含详细的说明文档，介绍您的代码所做的更改和新增功能。我们会尽快对您的提交进行审核和合并。
