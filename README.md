<p align="center">
    <a href="http://www.maxiaoqu.com/">
        <img width="300" src="http://www.maxiaoqu.com/maxiaoqu.png">
    </a>
</p>

<h2>
    vue-selecttree
    <h4>一个很好用的Vue多功能 树组件</h4>
</h2>

## 相关链接
- [gitHub地址](https://github.com/maxiaoqu/vue-selecttree-demo/)
- [案例地址](http://github.maxiaoqu.com/vue-selecttree/)
- [api文档](http://blog.maxiaoqu.com/packagesApi/)
- [vue组件地址](https://github.com/maxiaoqu/vue-selecttree/)
- [npmjs插件](https://www.npmjs.com/package/vue-selecttree/)

## 使用方法
```vue
<template>
    <vue-selecttree :data="data" :props="defaultProps"></vue-selecttree>
</template>
<script>
    import vueSelecttree from 'vue-selecttree';
    export default {
        data () {
            return {
                defaultProps: {
                    children: 'children',
                    label: 'label'
                },
                data: [{
                      label: "一级 1",
                      name: "一级 1 000",
                      children: [{
                          label: "二级 1-1",
                          name: "二级 1-1 000",
                          children: [{
                              label: "三级 1-1-1",
                              name: "三级 1-1-1 000"
                          }]
                      }]
                    },{
                        label: "一级 2",
                        name: "一级 2 000",
                        children: [{
                            label: "二级 2-1",
                            name: "二级 2-1 000",
                            children: [{
                                label: "三级 2-1-1",
                                name: "三级 2-1-1 000"
                            }]
                        }]
                    }]
            }
        }
    }
</script>
```

## 主要维护人员
|人员|github账号|头像|作者博客|作者网站|联系邮箱|
|---|---|---|---|---|---|
|码小趣|[maxiaoqu](https://github.com/maxiaoqu) |  ![](https://avatars1.githubusercontent.com/u/25891598?s=60&v=4)|http://blog.maxiaoqu.com|http://www.maxiaoqu.com|maxiaoqu@gmail.com

## 安装
```
npm install
```

## 运行
```
npm run serve
```

## 打包
```
npm run build
```

## 检查
```
npm run lint
```

## 文件结构
```shell
├── public...........................打包所需静态资源
└── src..............................存放文件的相关目录
    └── assets.......................项目静态资源
        └── treeData.json............树组件需要的数据
    ├── components...................模板组件
        └── treerows.vue.............树组件的渲染盒子组件
    ├── iconfont.....................阿里巴巴图标库（icon图标）的树组件用到
    ├── view.........................页面文件
        └──  SelectTree.vue..........树组件展示
    ├── APP.vue......................app.vue文件
    └── main.js......................配置（阿里巴巴图标库）在这里引入
```