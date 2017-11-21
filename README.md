# vue-IE9-
vue-cli所建项目支持ie9+ 使用es6语法报错解决办法 [vuex] vuex requires a Promise polyfill in this browser. 
解决方法:
<pre>
1.npm install --save-dev babel-polyfill
在webpack.config.js配置
module.exports = {
  entry: {
    app: ['babel-polyfill','./src/main.js']
  },
};
</pre>
