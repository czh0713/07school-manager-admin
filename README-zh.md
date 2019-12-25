# vue-admin-template

> 这是一个极简的 vue admin 管理后台。它只包含了 Element UI & axios & iconfont & permission control & lint，这些搭建后台必要的东西。

[线上地址](http://panjiachen.github.io/vue-admin-template)

[国内访问](https://panjiachen.gitee.io/vue-admin-template)

目前版本为 `v4.0+` 基于 `vue-cli` 进行构建，若你想使用旧版本，可以切换分支到[tag/3.11.0](https://github.com/PanJiaChen/vue-admin-template/tree/tag/3.11.0)，它不依赖 `vue-cli`。

## Extra

如果你想要根据用户角色来动态生成侧边栏和 router，你可以使用该分支[permission-control](https://github.com/PanJiaChen/vue-admin-template/tree/permission-control)

## 相关项目

- [vue-element-admin](https://github.com/PanJiaChen/vue-element-admin)

- [electron-vue-admin](https://github.com/PanJiaChen/electron-vue-admin)

- [vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template)

- [awesome-project](https://github.com/PanJiaChen/vue-element-admin/issues/2312)

写了一个系列的教程配套文章，如何从零构建后一个完整的后台项目:
- [nodejs vue-element-admin (实训1)](https://www.jianshu.com/p/aaf830870744)
- [nodejs vue-element-admin（实训续2）](https://www.jianshu.com/p/584ff2e485d5)
- [nodejs vue-element-admin（实训续3）](https://www.jianshu.com/p/64f711c68fef)
- [nodejs vue-element-admin（实训续4）](https://www.jianshu.com/p/2bcfad54d0ba)
- [nodejs vue-element-admin（实训续5）](https://www.jianshu.com/p/50d50ecd30fa)
- [nodejs vue-element-admin（实训续6）](https://www.jianshu.com/p/d40cbd483fea)


## Build Setup

```bash
# 克隆项目
git clone https://github.com/PanJiaChen/vue-admin-template.git

# 进入项目目录
cd vue-admin-template

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装以来，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 [http://localhost:9528](http://localhost:9528)

# 实现过程
# 一、
# 1.安装nodejs
# 2.安装git
# 3.下载vue-element-admin
# 4.下载projectname
# 5.连接数据库monodb
# 二、搭建学校管理模块
# 三、创建学院管理模块(关联学院和学校)
# 四、创建班级管理模块（关联前者）
# 五、关键学生管理模块（关联前者）
# 六、创建教师管理模块（关联老师、学院、学校）
# 附加、
# 1.创建课程管理模块（关联学生、学院、学校）
# 2.班级人数颜色区分标签
# 3.男女颜色标签
# 4.学生模块搜索栏
# 5.主页面学生人数自动统计

![输入图片说明](https://images.gitee.com/uploads/images/2019/1213/092330_c25e9bae_5545388.png "捕获.PNG")

# 参与制作

[hlz_Y](http://gitee.com/hlz_y)

[zhou_kai_hua](http://gitee.com/zhou_kai_hua)

[zjr_a](http://gitee.com/zjr_a)

[xhb_jing](https://gitee.com/xhb_jing)

[去年的牛肉](https://www.jianshu.com/search?q=去年的牛肉&page=1&type=note)

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build:prod

## 其它

```bash
# 预览发布环境效果
npm run preview

# 预览发布环境效果 + 静态资源分析
npm run preview -- --report

# 代码格式检查
npm run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```

更多信息请参考 [使用文档](https://panjiachen.github.io/vue-element-admin-site/zh/)

## Demo

![demo](https://github.com/PanJiaChen/PanJiaChen.github.io/blob/master/images/demo.gif)

## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

## License

[MIT](https://github.com/PanJiaChen/vue-admin-template/blob/master/LICENSE) license.

Copyright (c) 2017-present PanJiaChen
