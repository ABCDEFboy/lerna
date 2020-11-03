# 开始

```bash
# 给其中一个包添加单独的依赖
lerna add axios --scope=demo

# 再比如要给 all-connection-base 添加 element-ui
lerna add element-ui --scope=all-connection-base

# 链接本地的包
lerna bootstrap

# 删除packages 中的 node_modules
lerna clean
```

# 如何连接

再 `packages/demo` 下的 package.json 中有一行 `"dog": "0.0.2"`，就是通过这一行把 `dog` 连接到 `cat` 项目到

# 发布

当测试了没有问题，就可以直接在 dog 下用 `npm publish` 进行发布

# 初始化 lerna

```bash
# 这个项目已经初始化好了
cd lerna-app
lerna init
```
