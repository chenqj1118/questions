npm cache clean -f  清除缓存
npm config set registry http://registry.npm.taobao.org
npm config set registry https://registry.npmjs.org/
npm config set registry http://dev.bokesoft.com:28080
npm config set registry http://1.1.5.46:8081/nexus/repository/npm-boke-all/

yarn config set registry https://registry.npm.taobao.org -g 
yarn config set sass_binary_site http://cdn.npm.taobao.org/dist/node-sass -g

二、yarn和npm命令对比

```
npm init	yarn init	初始化项目
npm install	yarn	安装全部依赖
npm install react --save	yarn add react	安装某个依赖，保存到 dependencies
npm uninstall react --save	yarn remove react	移除某个依赖
npm install react --save-dev	yarn add react --dev	安装某依赖,保存到 devDependencies
npm update [package] --save	yarn upgrade [package]	更新生产环境某个依赖包
npm install axios --global	yarn global add axios	全局安装某个依赖
npm install --save axios vue-axios	yarn add axios vue-axios	同时下载多个依赖包
npm install [package]@[version]	yarn add [package]@[version]	安装指定版本的包
npm rebuild	yarn install --force	重新下载所有包
```

npm5版本之前，必须要加上--save，才会将包记录到package.json
npm5版本之后开始，--save是默认值了，可以省略不写

--save 简写 -S 会被记录到dependencies【生产环境】
npm	等同	yarn
npm i jquery // npm i jquery --save	=	yarn add jquery
npm i jquery -S	=	yarn add jquery -S // yarn 只有简写
--save-dev 简写 -D 会被记录到devDependencies【开发环境】
npm	等同	yarn
npm i webpack -D // npm i webpack --save-dev	=	yarn add webpack -D // yarn 只有简写
dependencies:项目依赖，项目实际运行需要的依赖，上线还是需要的，如（vue，jquery）
devDependencies:开发依赖，只在开发时需要的依赖，实际上线不需要的，如（webpack）

创建vue项目的方式：

1. npm init webpack my-app(vue-cli2)
2. vue create my-app            (vue-cli3)

创建react项目的方式：

1. npm init react-app my-app
   yarn create react-app my-app
2. npx create-react-app my-app
   bokests构建打包后，前端代码所在的jar里面的位置：
     \bokests-test\aaa\deploy\dee-integration-starter-aa\schemes\default\boke-dee-integration-starter-server-starter-1.0.0-SNAPSHOT\BOOT-INF\lib\dee-integration-runtime-5.0.0\static\index.html

  debugger // eslint-disable-line
  /* eslint-disable */
  /* eslint-enable */
  width: calc(100% - 240px);
  ["1","2","3"].map(x=>parseInt(x)); --> [1,2,3]
```
  every()：对数组中的每一项运行给定函数，如果该函数对每一项都返回true，则返回true。
  filter()：对数组中的每一项运行给定函数，返回该函数会返回true的项组成的数组。
  forEach()：对数组中的每一项运行给定函数。这个方法没有返回值。
  map()：对数组中的每一项运行给定函数，返回每次函数调用的结果组成的数组。
  some()：对数组中的每一项运行给定函数，如果该函数对任一项返回true，则返回true。124,861
  find():  函数用来查找目标元素，找到就返回该元素，找不到返回undefined。var v1 = arr.find((value, index, arr) => { return value > 4}) //返回单个item值
  findIndex():  函数也是查找目标元素，找到就返回元素的位置，找不到就返回-1  //返回number 值
```
