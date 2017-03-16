React Native总结
==

## 目录<br/>
* [NodeJs安装步骤](#NodeJs安装步骤)
    * nvm
    * npm
    * babel
<br/>
<br/>
<br/><br/>
<br/><br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/><br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
NodeJs安装步骤
-------------------------------------------------
nvm： 是NodeJs版本管理工具，可安装多个node版本进行管理。</br>
nvm配置淘宝镜像，修改settings.txt。</br>
root: D:\dev\nvm</br>
path: D:\dev\nodejs</br>
node_mirror: http://npm.taobao.org/mirrors/node/ </br>
npm_mirror: https://npm.taobao.org/mirrors/npm/</br>
	命令：</br>
		nvm install 6.10.0  安装node</br>
		nvm list            已安装node版本列表</br>
		nvm use 6.10.0      选中当前使用版本</br>

npm：是node安装后自带的工具，可以下载别人上传和自己上传的工具类。</br>
npm配置镜像：npm config set registry https://registry.npm.taobao.org</br>

babel：将ES6转化成ES5脚本。</br>
全局安装：npm install -g babel-cli</br>
使用npm创建一个nodejs工程：</br>
进入当前文件夹：npm init</br>
当前项目中安装转换插件工具（插件中的js代码，用于转换）</br>
     npm install babel-preset-es2015 –save</br>
手动将ES6转换成ES5（这个是在服务端替换）</br>
	 babel es6.js --out-file es5.js --presets es2015</br>
自动转换（直接将ES6下载到本地替换）</br>
		 babel es6.js -w --out-file es5.js --presets es2015</br>
在页面中实时转换，需要安装一个工具</br>
	npm install babel-core@5 –save</br>
使用Browsersync实时刷新页面（可以快速响应文件刷新界面）</br>
安装：npm install -g browser-sync</br>
在当前项目下启动Browsersync，开始监听：</br>
browser-sync start --server --files "**"</br>
访问时需要前面加上Local:http://localhost:3000</br>
