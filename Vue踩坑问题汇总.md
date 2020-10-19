npm install sass-loader --save-dev`

###### 在build文件夹下的webpack.base.conf.js的rules里面添加如下配置

```
{
test: /\.scss$/,
loaders: ['style', 'css', 'sass']
}
```

###### 基本上都是sass-loader的版本过高导致的编译错误,需要降低版本

解决方法：cd到项目文件下运行

```
npm uninstall sass-loader(卸载当前版本)

npm install sass-loader@7.0.3 --save-dev
```



#### 1.3 Vue启动问题(You may use special comments to disable some warnings.)

导致问题出现的原因：ESlint的监测机制

解决方法①：在build/webpack.base.conf.js文件中注释掉第43行代码，如下图，重新yarn start 或者npm run dev

![](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20200916154027871.png)



解决方法②：在config/index.js文件中第26行中的useEslint的值改为false，如下图，然后重新启动程序

![](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20200916154207464.png)



#### 1.4 端口号查询

##### 查看被占用的端口号：

netstat -ano | findstr 端口号

##### 杀死占用的端口号：

taskkill /pid 端口号 /f